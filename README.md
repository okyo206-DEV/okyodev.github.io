# YT Repeater Pro 公式サイト

GitHub Pages にデプロイするための公式サイトテンプレートです。

## 公開前に編集する項目

### 1. 購入リンク（`index.html`）

以下の2箇所のURLを Lemon Squeezy の実際のチェックアウトURLに置き換えてください。

```
https://YOUR-STORE.lemonsqueezy.com/checkout/buy/YOUR-PRODUCT-ID
```

Lemon Squeezy ダッシュボード → 商品 → 「View product page」からURLを取得できます。

### 2. デモ動画（`index.html`）

YouTubeの埋め込みURLの `YOUR_VIDEO_ID` を実際の動画IDに置き換えてください。

```
https://www.youtube.com/embed/YOUR_VIDEO_ID
```

### 3. メールアドレス（全ページ）

`support@yourdomain.com` を独自ドメインのメールアドレスに置き換えてください。

- `privacy.html`
- `terms.html`
- `about.html`
- `contact.html`

### 4. 日付（`privacy.html`, `terms.html`）

`[Date]` を実際の日付に置き換えてください（例：February 21, 2025）。

### 5. スクリーンショット

`screenshots/` フォルダに以下の画像を追加してください。

- `screenshot1.png` - メイン画面
- `screenshot2.png` - 機能画面
- `screenshot3.png` - 使用例

`index.html` の `screenshot-grid` 内の `src` パスが正しいか確認してください。

## GitHub Pages へのデプロイ手順

1. GitHub で新規リポジトリを作成
2. リポジトリ名を `yourusername.github.io` にする（ユーザーページの場合）
3. この `website` フォルダ内の全ファイルをリポジトリのルートにアップロード
4. Settings → Pages → Source: Deploy from a branch
5. Branch: main、フォルダ: / (root) で保存

## 独自ドメインの設定

1. Settings → Pages → Custom domain に `yourdomain.com` を入力
2. ドメインレジストラ（お名前.comなど）のDNSで以下を設定：
   - **Aレコード**（4つ）: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. DNS反映後（10分〜48時間）、Enforce HTTPS にチェック
