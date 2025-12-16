# iframe-check

iframe動作確認用の最小構成プロジェクト

## GitHub Pagesへのデプロイ手順

### 1. リポジトリをGitHubにプッシュ

```bash
# リポジトリを初期化（まだの場合）
git init

# ファイルを追加
git add .

# コミット
git commit -m "Initial commit: Add Hello World HTML"

# GitHubリポジトリを作成し、リモートを追加
# （GitHub上でリポジトリを作成後）
git remote add origin https://github.com/YOUR_USERNAME/iframe-check.git

# プッシュ
git branch -M main
git push -u origin main
```

### 2. GitHub Pagesを有効化

1. GitHubリポジトリのページにアクセス
2. **Settings** タブをクリック
3. 左サイドバーの **Pages** をクリック
4. **Source** セクションで：
   - **Branch** を選択
   - ブランチを `main` に設定
   - フォルダを `/ (root)` に設定
5. **Save** をクリック

### 3. デプロイ確認

数分待つと、以下のURLでアクセスできます：
```
https://YOUR_USERNAME.github.io/iframe-check/
```

### 4. iframeで確認

他のページから以下のようにiframeで埋め込んで動作確認できます：

```html
<iframe src="https://YOUR_USERNAME.github.io/iframe-check/" width="800" height="600"></iframe>
```

## ローカルで確認

```bash
# シンプルなHTTPサーバーで起動（Python 3の場合）
python3 -m http.server 8000

# ブラウザで http://localhost:8000 にアクセス
```
