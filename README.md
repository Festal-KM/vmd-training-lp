# VMD実践研修 LP（株式会社 Grow Up Job）

携帯電話 催事営業向け VMD実践研修プログラムのランディングページです。

## 構成
- `index.html` — LP本体（単一ページ）
- `assets/cover-hero.png` — ヒーロー背景写真

## GitHub Pages で公開する手順

### 方法A：ブラウザだけで完結
1. このリポジトリの「Add file → Upload files」を開く
2. `index.html` と `assets/` フォルダ（`cover-hero.png` を含む）をアップロードしてコミット
3. リポジトリの **Settings → Pages** を開く
4. **Build and deployment → Source** を「Deploy from a branch」に設定
5. **Branch** を `main` / フォルダ `/ (root)` にして Save
6. 数十秒〜数分後、`https://takahiro5757.github.io/-Training-business_lp/` で公開されます

### 方法B：ローカルから git で push
```bash
git clone https://github.com/takahiro5757/-Training-business_lp.git
cd -Training-business_lp
# この deploy フォルダの中身（index.html と assets/）をここにコピー
git add .
git commit -m "Add VMD training LP"
git push origin main
```
その後、方法Aの手順3以降で GitHub Pages を有効化してください。

## 注意
- `index.html` は `assets/cover-hero.png` を相対パスで参照しています。**`assets` フォルダごと** 同じ階層に置いてください。
- フォント（Google Fonts）はCDNから読み込むため、公開環境ではインターネット接続が必要です。
