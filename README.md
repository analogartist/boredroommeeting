# boredroommeeting.com

Blog. Static HTML. Hosted on GitHub Pages.

## Setup

1. Create a GitHub repo named `boredroommeeting`
2. Push this code
3. Go to Settings → Pages → Source: Deploy from branch → `main` / `/ (root)`
4. Add custom domain: `boredroommeeting.com`
5. In your DNS provider, add:
   - A records pointing to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Or a CNAME record: `www` → `analogartist.github.io`
6. Wait for DNS propagation and HTTPS certificate (can take up to 24 hours)
