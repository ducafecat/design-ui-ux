# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | 日本語 | [한국어](README.ko.md) | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

HTML + Tailwind で UI/UX プロトタイプを作成します。デザイン参考の検索、スタイルの選択から、ブラウザーでプレビューできるページの作成まで進められます。

## インストール

npx でインストールします。プロジェクト内へのインストールを推奨します。

```bash
npx skills add ducafecat/design-ui-ux
```

## 使い方

### 1. デザイン参考を探す

作成するもの、対象ユーザー、必要な画面をまとめた製品要件定義書（PRD）を用意し、次のように入力します。

```text
/design-ui-ux 小紅書（Xiaohongshu）風のモバイル UI をデザインしてください。

参考：
docs/prd.md
```

![デザイン方向の検索](images/1795618228981.png)

### 2. デザインの方向性を選ぶ

検索結果から好みの方向性を選びます。候補が合わなければ、追加を依頼できます。

```text
別の候補を見せてください。
```

![デザイン方向の選択](images/1795618428611.png)

### 3. プロトタイプを作成する

選んだ参考の番号（例：B2）を入力します。その後、提示されたスタイルから選択します。たとえば、1 番を選びます。

![参考を選択し、スタイルの選択肢を確認します。](images/1795618786169.png)

```text
B2
```

![参考を選択し、スタイルの選択肢を確認します。](images/1795619134358.png)

1 番を選ぶ例：

```text
1
```

確認後、プロトタイプは `design/index.html` に保存されます。ブラウザーで開いて確認してください。

![完成したプロトタイプ](images/1795620741606.png)

### 4. 画面を並べて表示する

複数の画面をまとめて確認するには、次のように入力します。

```text
design/index.html の各画面を横に並べて、design/平铺.html に保存してください。
```

保存先： `design/平铺.html`

![画面の一覧](images/1795620965224.png)

### 5. 複数の案を比較する

スタイルを決めきれない場合は、それぞれのホーム画面を作成して比較できます。

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

## フィードバック・メンテナンス・ライセンス

改善を送る前に [CONTRIBUTING.md](CONTRIBUTING.md) をお読みください。変更履歴は [CHANGELOG.md](CHANGELOG.md)、機密性のある問題は [SECURITY.md](SECURITY.md) を参照してください。再現可能な問題は [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues) に報告できます。

このプロジェクトには、まだライセンスが指定されていません。利用・再配布前に必要な許諾を確認してください。公開前に、メンテナーはコードとデータの出典、再配布権、ライセンスを確認する必要があります。出典の記載だけでは再配布の許可を意味しません。[出典に関する注意事項](NOTICE.md) を参照してください。
