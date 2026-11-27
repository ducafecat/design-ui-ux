# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | 日本語 | [한국어](README.ko.md) | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

コーディング支援ツール向けの UI/UX デザインスキルです。参考例とスタイルを選び、要件を HTML + Tailwind のプロトタイプにまとめます。完成したファイルはブラウザーで開いて確認できます。

## インストール

プロジェクトのフォルダーで実行します。

```bash
npx skills add ducafecat/design-ui-ux
```

## 使い方

### 1. デザイン参考を探す

何を作るか、誰が使うか、どの画面が必要かを伝えます。要件定義書（PRD）があれば、ファイルのパスを添えてください。

```text
/design-ui-ux 小紅書（Xiaohongshu）風のモバイル UI をデザインしてください。

参考：
docs/prd.md
```

![デザイン方向の検索](images/1795618228981.png)

### 2. デザインの方向性を選ぶ

気に入った参考例を選びます。合うものがなければ、別の候補を頼めます。

```text
別の候補を見せてください。
```

![デザイン方向の選択](images/1795618428611.png)

### 3. プロトタイプを作成する

選んだ参考例の番号を返信します。たとえば：

![参考例の選択](images/1795618786169.png)

```text
B2
```

続いてスタイルを選びます。

![スタイルの選択肢](images/1795619134358.png)

最初の選択肢なら、次のように返信します。

```text
1
```

確認後、プロトタイプは `design/index.html` に保存されます。ブラウザーで開いて確認してください。

![完成したプロトタイプ](images/1795620741606.png)

### 4. 画面を並べて表示する

各画面を一枚に並べてもらうこともできます。

```text
design/index.html の各画面を横に並べて、design/平铺.html に保存してください。
```

保存先： `design/平铺.html`

![画面の一覧](images/1795620965224.png)

### 5. 複数の案を比較する

迷ったら、スタイルごとにホーム画面を作って比べてみてください。

```text
選択肢 1、2、3、4 のホーム画面をそれぞれ作成し、design/compare.html に保存してください。
```

保存先： `design/compare.html`

![4つのデザイン案](images/1795619938511.png)

## 動作要件

- インストールには Node.js 22.20 以降と npm / npx が必要です。生成された HTML の表示に Node.js は不要です。
- ローカルデータ検索には Python 3 が必要です。外部パッケージは不要です。Python がなくてもデザイン指針に沿って作成できますが、ローカル検索は使えません。
- 参考の検索と画面確認には、スクリーンショットとローカル HTML のプレビューに対応したブラウザーが必要です。既定は Ego Lite で、`ego-browser` スキルを別途設定します。スキルの説明に従い、他のブラウザーも利用できます。
- 作成時には Tailwind のコンパイルが必要です。納品前にコンパイルし、最終 HTML を Node.js、CDN、実行時ビルドなしで開けるようにします。

## フィードバックとライセンス

改善を送る前に [CONTRIBUTING.md](CONTRIBUTING.md) をお読みください。変更履歴は [CHANGELOG.md](CHANGELOG.md)、機密性のある問題は [SECURITY.md](SECURITY.md) を参照してください。再現可能な問題は [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) に報告できます。

このプロジェクトは [MIT ライセンス](LICENSE) で提供されます。第三者のコード、データ、フォント、画像などには、それぞれのライセンスが適用されます。上流プロジェクトのクレジットと出典は [NOTICE.md](NOTICE.md) を参照してください。
