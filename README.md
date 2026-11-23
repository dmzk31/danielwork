# danielwork｜Three.js 3D 工作島

使用 Three.js 製作的 Low-poly 3D 工作島；一座小島含六個工作區域，對應原 Google Sites 的 **43 個第一層連結**。

## 已完成

- 純 Three.js Geometry 建模：漂浮島嶼、海洋、道路、樹木、廣場、辦公中心、校舍、活動中心、旅行碼頭、玻璃學習館、生活小屋。
- **無教堂、十字架或任何宗教造型／裝飾**。分類名稱與超連結保留原 Google Sites 內容。
- 滑鼠拖曳旋轉、滾輪縮放；手機單指旋轉、雙指縮放。
- 點擊 3D 建築或導覽標籤，顯示對應分類的所有連結。
- 搜尋 43 個第一層連結，點擊於新分頁開啟。
- 支援手機版、重設全景與使用者偏好減少動態效果。

## GitHub Pages 部署

1. 在 GitHub 新建**名稱為 `danielwork`** 的 Repository（如帳號允許公開，先確認是否含私人資料連結）。
2. 將本資料夾的 `index.html`、`css/`、`data/`、`.nojekyll` 和 `README.md` 上傳到 **main** 分支根目錄。
3. 進入 **Settings → Pages → Build and deployment**，設定 **Source: Deploy from a branch**、**Branch: main**、**Folder: /(root)**，儲存。
4. 網址格式：`https://你的-GitHub-帳號.github.io/danielwork/`。

本專案使用 Three.js `0.187.0` 的 CDN（jsDelivr），**無需 npm、無需後端、無需 API Key**。初次打開需有網路連線。部分瀏覽器直接以 `file://` 開啟可能有限制，建議透過 GitHub Pages 檢視。

## 修改連結

開啟 `data/links.js`，修改相對應的 `title` (顯示文字) 或 `url` (目的網址)，儲存並重新上傳即可。不要修改 `id`，否則建築無法對應到分類。

## 資料與隱私提醒

GitHub Public Repository 中的 `data/links.js` 可以被任何人閱讀。此版本依來源網站保留 43 個入口，包含個人紀錄類型的連結；**正式公開前請逐一檢查個人連結是否適合公開，並確認 Google Drive／表單原本的存取權限**。本網站本身不會繞過 Google 的存取控制。

來源頁面：`https://sites.google.com/view/danielwork/首頁`（2026-11-24 擷取公開連結；連結能否成功登入及使用，仍取決於原服務與權限）。

## 技術

Three.js + OrbitControls（同版本 ESM CDN）、原生 HTML / CSS / JavaScript、無建置工具、無外部 3D 模型、無外部圖片素材。
