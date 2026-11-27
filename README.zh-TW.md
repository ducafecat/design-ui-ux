# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | 繁體中文 | [日本語](README.ja.md) | [한국어](README.ko.md) | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

使用 HTML + Tailwind 製作 UI/UX 原型。從尋找設計參考、選擇風格，到產生可在瀏覽器中預覽的頁面，依照以下步驟即可開始。

[貓哥 Flutter 影片學習站](https://ducafecat.com/)

[Flutter 套件站](https://flutter.ducafecat.com/)

## 安裝

透過 npx 安裝，建議安裝至目前的專案：

```bash
npx skills add ducafecat/design-ui-ux
```

## 使用流程

### 1、尋找設計參考

建議先準備一份產品需求文件（PRD），說明要製作什麼、目標使用者，以及需要哪些頁面。接著輸入：

```text
/design-ui-ux 設計一個小紅書風格的行動版介面

參考
docs/prd.md
```

![自動搜尋設計方向](images/1795618228981.png)

### 2、選擇設計方向

從搜尋結果中挑選喜歡的方向。如果這批都不合適，可以繼續輸入：

```text
再換一批
```

![選擇設計方向](images/1795618428611.png)

### 3、產生設計稿

<img src="images/1795618786169.png" alt="提示" style="zoom: 50%;" />

輸入選中的參考編號，例如：

```text
B2
```

接下來會提供具體的風格選項，選擇符合預期的一項：

<img src="images/1795619134358.png" alt="設計風格" style="zoom:50%;" />

例如，選擇第 1 項：

```text
1
```

確認後，設計稿會儲存至 `design/index.html`，可在瀏覽器中開啟預覽。

<img src="images/1795620741606.png" alt="完成的設計稿" />

### 4、平鋪設計稿

想將各個頁面放在一起查看，可以輸入：

```text
將設計稿 design/index.html 平鋪排列，儲存至 design/平铺.html
```

結果儲存至 `design/平铺.html`：

![設計稿平鋪排列](images/1795620965224.png)

### 5、比較多個方案

不確定要選哪種風格時，可以請它分別製作一版首頁，放在一起比較：

```text
1 2 3 4 各製作一個首頁設計，儲存至 design/compare.html
```

結果儲存至 `design/compare.html`：

![四種首頁設計方案](images/1795619938511.png)

## 環境需求

- 安裝時需要 Node.js 22.20 或更新版本，以及 npm / npx。產生的 HTML 頁面不需要 Node.js。
- 本機資料檢索需要 Python 3，無須安裝第三方套件。沒有 Python 時，仍可依設計規範製作頁面，但無法使用本機檢索。
- 尋找參考和檢查頁面需要支援實際截圖與本機 HTML 預覽的瀏覽器。預設使用 Ego Lite，須另外設定 `ego-browser` 技能；也可依技能說明使用其他瀏覽器。
- 製作頁面時需要編譯 Tailwind。交付前應完成編譯，讓最終 HTML 無須 Node.js、CDN 或執行階段建置即可開啟。

## 意見回饋、維護與授權

提交改善前請閱讀 [CONTRIBUTING.md](CONTRIBUTING.md)，版本紀錄請見 [CHANGELOG.md](CHANGELOG.md)，敏感問題請見 [SECURITY.md](SECURITY.md)。可透過 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) 回報可重現的問題。

本專案目前尚未指定授權條款。使用或散布前，請確認相關授權；維護者也須在發布前核實程式碼與資料的來源、再散布權利及授權條款。資料中標示來源，不代表已取得再散布許可，詳見[來源說明](NOTICE.md)。
