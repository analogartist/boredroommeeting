# Context for Claude Code Session

## What this is
A static blog site for boredroommeeting.com, ready to deploy to GitHub Pages.

## Files (all in this directory)
- `index.html` — Homepage listing blog posts
- `drawing-as-input.html` — First blog post: "Why Can't I Just Draw Something and Have AI Understand It?"
- `CNAME` — GitHub Pages custom domain config pointing to boredroommeeting.com
- `README.md` — Setup instructions

## What needs to happen
1. Create a new GitHub repo under `analogartist` account (Susheel's GitHub username)
2. Push all files from this directory to `main` branch
3. Enable GitHub Pages: Settings → Pages → Source: `main` / `/ (root)`
4. Configure DNS for boredroommeeting.com:
   - A records → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Or CNAME `www` → `analogartist.github.io`
5. Enable HTTPS in GitHub Pages settings after DNS propagates

## Design
- Dark theme, editorial aesthetic
- Fonts: Instrument Serif (headings), DM Sans (body), JetBrains Mono (code)
- Accent color: #d4622b (burnt orange)
- Static HTML, no build step, no dependencies

## Background
This blog post was written during a live session exploring how to make drawing a first-class input modality for AI. The post documents the exploration — from trying to get Claude to see an Excalidraw canvas, to discovering that the real missing primitive is "temporal fusion" (simultaneous drawing + voice as a single timestamped input stream to an LLM). Nobody has built this yet.
