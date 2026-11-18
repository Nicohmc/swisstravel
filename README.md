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


## V2 — 整張圓形城鎮圖片都可點擊

地圖上七個城鎮的**插畫圓形照片**現在是透明的互動按鈕，不再需要對準原本的小圓點。滑鼠滑過會出現高亮外框及 VIEW TOWN，選取會保留橙色圓環。點選後，資訊、注意事項、私人筆記及匯入／匯出功能皆維持原樣。手機點擊後會捲動至資訊面板。

### 自訂按鈕位置

若更換底圖，可編輯 `script.js` 裡 `TOWNS` 的 `x`、`y`、`diameter`：
- `x`：圓形照片中心點，佔圖片寬度的百分比。
- `y`：圓形照片中心點，佔圖片高度的百分比。
- `diameter`：照片圓的直徑，佔圖片寬度的百分比。

此版位置是依照專案內 `assets/winter-map.png`（1055 × 1491 像素）調整。

### 更新 GitHub Pages

將此資料夾中的 `index.html`、`style.css`、`script.js` 和 `assets/winter-map.png` 上傳覆蓋原檔，或直接保留圖片、僅替換前三個檔案。

筆記使用既有的 `swiss-winter-notes-v1` localStorage key，原瀏覽器資料可繼續使用；保險起見，可先從舊版網站匯出筆記 JSON 做備份。

## V3 — Glowing arrows, invisible circular hit areas

The orange circular outlines and VIEW TOWN badge have been removed. Each illustrated town now shows a glowing blue-white arrow, but the **entire original circular photo** remains a clickable button. On hover/focus the arrow brightens; the selected town keeps a brighter arrow. All data and note storage are unchanged.

To adjust arrow styling, edit `.town-photo::after` in `style.css`. To adjust the clickable circle size and position, edit `x`, `y`, `diameter` in `script.js`.
