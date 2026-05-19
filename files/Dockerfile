FROM nginx:alpine

# Remove default nginx static assets
RUN rm -rf /usr/share/nginx/html/*

# Copy our site
COPY index.html /usr/share/nginx/html/
COPY privacy.html /usr/share/nginx/html/
COPY terms.html /usr/share/nginx/html/
COPY robots.txt /usr/share/nginx/html/
COPY sitemap.xml /usr/share/nginx/html/

# Custom nginx config (handles Railway's dynamic PORT)
COPY nginx.conf /etc/nginx/templates/default.conf.template

# Railway injects PORT env var; nginx:alpine processes templates on start
ENV PORT=8080

EXPOSE 8080

CMD ["nginx", "-g", "daemon off;"]
