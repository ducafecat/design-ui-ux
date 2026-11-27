# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | 繁體中文 | [日本語](README.ja.md) | [한국어](README.ko.md) | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

一個給程式開發助手使用的 UI/UX 設計技能。先看參考、選風格，再將需求做成 HTML + Tailwind 原型，用瀏覽器開啟就能查看。

[貓哥 Flutter 影片學習站](https://ducafecat.com/)

[Flutter 套件站](https://flutter.ducafecat.com/)

## 安裝

在專案目錄中執行：

```bash
npx skills add ducafecat/design-ui-ux
```

## 使用流程

### 1、尋找設計參考

說明要做什麼、給誰用、需要哪些頁面。如果已有產品需求文件（PRD），可以直接附上路徑：

```text
/design-ui-ux 設計一個小紅書風格的行動版介面

參考
docs/prd.md
```

![自動搜尋設計方向](images/1795618228981.png)

### 2、選擇設計方向

挑一個喜歡的參考。都不適合就請它再找一批：

```text
再換一批
```

![選擇設計方向](images/1795618428611.png)

### 3、產生設計稿

<img src="images/1795618786169.png" alt="提示" style="zoom: 50%;" />

回覆參考編號，例如：

```text
B2
```

再從提供的風格中選一個：

<img src="images/1795619134358.png" alt="設計風格" style="zoom:50%;" />

選第 1 項就回覆：

```text
1
```

確認風格後，技能會開始製作，設計稿儲存在 `design/index.html`。用瀏覽器開啟即可查看與操作。

<img src="images/1795620741606.png" alt="完成的設計稿" />

### 4、平鋪設計稿

想把幾個頁面放在一起看，可以這樣說：

```text
將設計稿 design/index.html 平鋪排列，儲存至 design/平铺.html
```

開啟 `design/平铺.html`，一起查看各個頁面：

![設計稿平鋪排列](images/1795620965224.png)

### 5、比較多個方案

還沒決定風格？可以各做一版首頁再比較：

```text
1 2 3 4 各製作一個首頁設計，儲存至 design/compare.html
```

開啟 `design/compare.html` 比較各個方案：

![四種首頁設計方案](images/1795619938511.png)

## 環境需求

- **安裝：** Node.js 22.20 或更新版本，以及 npm / npx。查看完成的 HTML 不需要 Node.js。
- **本機檢索：** Python 3，不需額外套件。沒有 Python 也能依設計規範製作頁面，只是無法搜尋本機資料。
- **瀏覽器：** 需要支援截圖和本機 HTML 預覽。預設使用 Ego Lite，請先另外設定 `ego-browser` 技能；其他瀏覽器的用法見技能說明。
- **Tailwind：** 製作時需要編譯樣式。交付前完成編譯，最終 HTML 應能直接開啟，無須 Node.js、CDN 或執行階段建置。

## 回饋與授權

提交改善前請閱讀 [CONTRIBUTING.md](CONTRIBUTING.md)，版本紀錄請見 [CHANGELOG.md](CHANGELOG.md)，敏感問題請見 [SECURITY.md](SECURITY.md)。可透過 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) 回報可重現的問題。

本專案採用 [MIT 授權條款](LICENSE)。第三方程式碼、資料、字型、圖片及其他素材仍適用各自的授權條款。上游署名與來源紀錄請見 [NOTICE.md](NOTICE.md)。
