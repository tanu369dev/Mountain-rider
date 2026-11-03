# Singletrack Exchange

A website for buying and selling used mountain bikes. It is one file (`index.html`) with no build step and no dependencies to install.

## What it does

- Browse bikes in a grid and filter by type of riding, max price (₹), wheel size, frame size, suspension and condition
- Search, sort, and save bikes with a heart
- Open a bike to see its specs, description and seller contact
- Sell a bike with a form (photo optional) and a live preview card
- An animated motorbike rides into the opening page (tap it to replay)
- Light and dark themes follow the visitor's device settings

## Run it on your computer

Double-click `index.html`. It opens in your browser.

## Put it on GitHub and publish it for free (GitHub Pages)

1. Go to https://github.com/new and create a repository, for example `singletrack-exchange`. Choose Public.
2. On the new repository page, click **uploading an existing file**.
3. Drag in `index.html` and `README.md`, then click **Commit changes**.
4. Open **Settings**, then **Pages**.
5. Under **Build and deployment**, set Source to **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then click **Save**.
6. After a minute or two, your site is live at `https://YOUR-USERNAME.github.io/singletrack-exchange/`.

Using git from a terminal instead:

```bash
cd singletrack-exchange
git init
git add index.html README.md
git commit -m "Add Singletrack Exchange"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/singletrack-exchange.git
git push -u origin main
```

## Important: listings are saved per browser

The eight bikes marked "Sample" are made-up examples. When someone posts a bike on this static version, it is stored only in that visitor's own browser (localStorage), so other visitors will not see it.

To make listings shared between everyone, the site needs a backend, such as Supabase or Firebase, to store listings and photos. In `index.html`, the functions `submitListing` and the `db` block near the end of the script are where that would plug in.

## Files

- `index.html`: the whole site (HTML, CSS and JavaScript)
- `README.md`: this file

Fonts (Big Shoulders Display, Figtree, IBM Plex Mono) load from Google Fonts. Without internet, the page falls back to system fonts.
