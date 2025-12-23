# GitHub アップロード手順

## リポジトリの設定

1. GitHubで新しいリポジトリを作成
   - リポジトリ名: `RPGMapEditor`
   - 公開設定: Public
   - README: 追加しない（既存のものを使用）

2. ローカルリポジトリにリモートを追加
```bash
cd D:\RPGMakerMZ\RPGMapEditor
git remote add origin https://github.com/YOUR_USERNAME/RPGMapEditor.git
```

3. プッシュ
```bash
git push -u origin master
```

## 認証方法

GitHubの認証には以下の方法があります：

### Personal Access Token (推奨)
1. GitHub Settings → Developer settings → Personal access tokens
2. Generate new token (classic)
3. repoスコープを選択
4. git pushの際にパスワードの代わりにトークンを使用

### GitHub CLI
```bash
gh auth login
```

## 注意事項

- トークンは安全に管理してください
- コミット履歴にトークンを含めないでください
- 定期的にトークンを更新することを推奨します