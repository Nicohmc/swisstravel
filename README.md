# Swiss Winter Towns — Interactive Map

A static GitHub Pages website with seven clickable towns on an illustrated Swiss winter map.

## Publish on GitHub Pages

1. Create a public GitHub repository, e.g. `swiss-winter-towns`.
2. Upload `index.html`, `style.css`, `script.js` and the `assets` folder to the **repository root**.
3. Go to **Settings → Pages → Build and deployment → Deploy from a branch**.
4. Choose **main** and **/(root)**, then click **Save**.
5. Visit the URL GitHub Pages shows (usually `https://YOURNAME.github.io/swiss-winter-towns/`).

## Customize

- Change the town descriptions, tips, walking spots, travel times and pin coordinates in the `TOWNS` array at the top of `script.js`.
- Replace `assets/winter-map.png` with another poster if desired; adjust x/y percentages accordingly.
- Personal notes entered in the website are stored **only in that browser** using localStorage. They do **not** sync to GitHub or across devices. Use **Export notes JSON** to back them up, and **Import notes** to restore them.
- Do not put private notes in `script.js` or other published files unless you intend to make them public.
- The illustrated map is decorative and not geographically exact. Train times are estimates; check SBB before travel.

No build tools, accounts, frameworks or backend are needed.
