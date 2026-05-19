# Elite Team Sports

A members-only batting cage facility website. Built by Programmatic Partners.

**Live site:** https://eliteteamsportsms.com

## Stack

- Static HTML / CSS / JS (no build step)
- Nginx (alpine) for serving
- Deployed on Railway

## Local development

Open `index.html` directly in a browser, or run a local server:

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

## Deployment

Push to `main` on GitHub. Railway is connected to this repo and auto-deploys
on every push using the included `Dockerfile`.

## Files

- `index.html` - Homepage
- `privacy.html` - Privacy Policy
- `terms.html` - Terms of Service
- `robots.txt` - Search engine directives
- `sitemap.xml` - Site map for search engines
- `Dockerfile` - Container build instructions
- `nginx.conf` - Nginx server config
- `railway.json` - Railway deployment config

## Contact

500 Wilkins Wise Rd, Columbus, MS
