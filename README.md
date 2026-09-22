# Portfolio — GitHub Pages setup

This is a single self-contained page (fonts load from Google Fonts; all images are embedded, so there are no other assets to upload).

## Steps

1. Create a new repository on GitHub — for a personal site, name it exactly:
   `your-username.github.io`
   (Any other name works too, but your site's URL will then be `your-username.github.io/repo-name` instead of the root domain.)

2. Upload `index.html` to the root of that repository.
   - Via the GitHub website: open the repo → **Add file → Upload files** → drag in `index.html` → **Commit changes**.
   - Or via git:
     ```
     git clone https://github.com/your-username/your-username.github.io.git
     cd your-username.github.io
     cp /path/to/index.html .
     git add index.html
     git commit -m "Add portfolio"
     git push
     ```

3. Turn on Pages:
   - Go to the repo's **Settings → Pages**.
   - Under "Build and deployment", set **Source** to **Deploy from a branch**.
   - Set **Branch** to `main` (or `master`) and folder to `/ (root)`, then **Save**.

4. Wait a minute or two, then visit:
   - `https://your-username.github.io` (if you used the special repo name), or
   - `https://your-username.github.io/repo-name` (for any other repo name)

## Custom domain (optional)

If you own a domain, add it under **Settings → Pages → Custom domain**, then create a `CNAME` record at your DNS provider pointing to `your-username.github.io`.

## Updating later

Any time you want to change the content, edit `index.html` and push/upload the new version — GitHub Pages redeploys automatically within a minute or two.
