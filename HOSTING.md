# Hosting Dover Porchfest on GitHub Pages

This gets your site live at **https://jthmiller.github.io/porchfest** in about 5 minutes.

---

## Option A — Upload via GitHub.com (no coding needed)

1. Go to **https://github.com/jthmiller** and click **"New"** (green button, top right)
2. Name the repo: `porchfest`
3. Set it to **Public**, then click **"Create repository"**
4. On the next screen, click **"uploading an existing file"**
5. Drag and drop `index.html` into the window → click **"Commit changes"**
6. Go to **Settings → Pages** (left sidebar)
7. Under "Branch", select `main` and `/ (root)` → click **Save**
8. Done! Your site will be live at **https://jthmiller.github.io/porchfest** within ~60 seconds.

---

## Option B — Via Git command line

```bash
# Clone your new repo (create it on GitHub first as above)
git clone https://github.com/jthmiller/porchfest
cd porchfest

# Copy index.html into the folder
cp /path/to/index.html .

# Push it up
git add index.html
git commit -m "Add Porchfest app"
git push origin main
```

Then enable Pages in **Settings → Pages → Branch: main → Save**.

---

## Share the link

Once live, share: **https://jthmiller.github.io/porchfest**

Works on mobile, no app install needed.

---

## Want to update the map embed?

The Google Maps embed in the page is a placeholder. To add a real custom map:

1. Go to **https://www.google.com/maps/d/** and create a "My Map"
2. Add pins for all 11 porch locations
3. Click **Share → Embed** and copy the `<iframe>` src URL
4. In `index.html`, find the `<iframe class="map-embed"` line and replace the `src="..."` value
