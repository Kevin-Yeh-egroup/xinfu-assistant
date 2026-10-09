# 創業貸款準備助手（信扶專案）

靜態網站，由 Vercel 從這個 repo 自動部署。

| 網址 | 內容 |
|---|---|
| `/` | 引導員版 |
| `/review` | 審查人員版（第一次使用要輸入審查通行碼） |
| `/videos/guide.mp4`、`/videos/reviewer.mp4` | 教學影片 |

- 填寫的資料只存在使用者自己的瀏覽器，網站不收任何資料；頁面不連外、沒有分析追蹤。
- 不讓搜尋引擎收錄（`X-Robots-Tag: noindex`）。

## 更新內容

審查人員在「維護內容」修改作業說明或 AI 審核注意事項後，會匯出新的 HTML：

- 引導員版 → 取代 `index.html`
- 審查人員版 → 取代 `review/index.html`

推上 `main` 後，Vercel 會自動重新部署。
