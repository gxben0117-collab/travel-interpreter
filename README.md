# 旅途口譯

日本、韓國旅行用的面對面語音翻譯網頁（中文 ⇄ 日文／韓文）。

- 正式站：https://gxben0117-collab.github.io/travel-interpreter/
- 單檔 `index.html`，無建置步驟；改完 commit + push 到 main 即更新 GitHub Pages。
- 語音辨識：瀏覽器 Web Speech API（iPhone 用 Safari、Android 用 Chrome）。
- 翻譯：Anthropic API（瀏覽器直連，`anthropic-dangerous-direct-browser-access`）；金鑰只存在使用者手機的 localStorage，程式碼裡沒有金鑰。
- 模型：預設 `claude-haiku-5-5`（快），可切 `claude-sonnet-5-5`；effort low + JSON schema 結構化輸出。
- 上半部 `rotate(180deg)` 給對面的人看，兩邊各有麥克風鈕。
- `artifact版/`：最早發布在 Claude Artifact 的版本（無麥克風權限，已不再維護）。
