# The Fellowship Garage — fsg.vardon.org

Static site for the Freedom Center Church summer group (classic car restoration fundraiser for Kingdom Builders).

## Structure
- `index.html` — the whole site (single file, no build step)
- `updates.json` — build log entries (newest first). Add an object `{date, title, body}` to post an update.
- `photos.json` — gallery manifest: `[{"file":"name.jpg","caption":"..."}]`; put images in `photos/`
- `img/logo.png` — group logo

## Deploy
Served by nginx on CT385 (10.0.0.x:80) behind the Brain Cloudflare tunnel → https://fsg.vardon.org
Deploy: push to main → `POST https://gateway.infinihash.com/deploy/fellowship-garage`
