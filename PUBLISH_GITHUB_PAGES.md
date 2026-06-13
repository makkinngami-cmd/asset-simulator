# GitHub Pages公開手順

このフォルダはGitリポジトリ初期化済みです。
GitHub CLIのログイン後、以下で公開できます。

## 1. GitHub CLIにログイン

```powershell
gh auth login
```

## 2. Gitユーザー情報を未設定なら設定

```powershell
git config --global user.name "makki"
git config --global user.email "GitHubに登録しているメールアドレス"
```

ローカルだけで設定する場合:

```powershell
git config user.name "makki"
git config user.email "GitHubに登録しているメールアドレス"
```

## 3. リポジトリ作成、push、Pages有効化

```powershell
gh repo create asset-simulator --public --source . --remote origin --push
gh api repos/:owner/asset-simulator/pages -X POST -f source.branch=main -f source.path=/
gh repo view asset-simulator --web
```

Pagesの公開URLは通常以下です。

```text
https://<github-user>.github.io/asset-simulator/
```

## 補足

`gh api .../pages` が既に有効化済みで失敗する場合は、GitHubの `Settings > Pages` で `main` / root を指定してください。
