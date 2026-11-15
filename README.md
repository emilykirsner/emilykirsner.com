# Emily Kirsner portfolio site

A single-page site: `index.html` is the whole site (images are built in). Fonts load from Google Fonts.

## Put it online with GitHub Pages (free, no command line)

1. Create a free account at github.com, then click **New repository**.
   - Name it `emilykirsner-site` (any name works).
   - Set it to **Public** (GitHub Pages on free accounts publishes from public repositories).
2. In the new repo, click **Add file > Upload files**. Drag in everything from this folder
   (`index.html`, `.nojekyll`, and the `videos` folder), then click **Commit changes**.
3. Go to **Settings > Pages**. Under **Build and deployment**, set Source to
   **Deploy from a branch**, Branch **main**, folder **/ (root)**, and Save.
4. After a minute or two your site is live at `https://YOUR-USERNAME.github.io/emilykirsner-site/`.

## Use your own domain (emilykirsner.com)

1. Buy the domain from a registrar (Cloudflare, Namecheap, Porkbun, Squarespace and others work).
2. In your repo go to **Settings > Pages > Custom domain**, type `emilykirsner.com`, and Save.
   (Do this before changing DNS. GitHub also recommends verifying the domain under your
   account's Pages settings to prevent anyone else claiming it.)
3. At your registrar's DNS settings add these records:

   | Type  | Name | Value |
   |-------|------|-------|
   | A     | @    | 185.199.108.153 |
   | A     | @    | 185.199.109.153 |
   | A     | @    | 185.199.110.153 |
   | A     | @    | 185.199.111.153 |
   | AAAA  | @    | 2606:50c0:8000::153 |
   | AAAA  | @    | 2606:50c0:8001::153 |
   | AAAA  | @    | 2606:50c0:8002::153 |
   | AAAA  | @    | 2606:50c0:8003::153 |
   | CNAME | www  | YOUR-USERNAME.github.io |

   The CNAME points to your username only, without the repo name. The AAAA rows are optional.
   Don't add wildcard (*) records.
4. DNS can take from a few minutes to a few hours. When GitHub finishes, tick
   **Enforce HTTPS** in Settings > Pages.
5. With both records set up, `www.emilykirsner.com` redirects to `emilykirsner.com` automatically.

## Updating the site

Edit `index.html` in GitHub (pencil icon) or upload a new copy with **Add file > Upload files**.
The site refreshes within a couple of minutes.

## Adding videos

See `videos/README.txt`.

Records and settings above follow GitHub's current Pages documentation. If anything looks
different on screen, GitHub's docs at docs.github.com/pages are the source of truth.
