# Love_Common_test

2025ステージ班　恋愛共通テスト　進捗管理用

## 🚀 使い方

### 開発環境の起動
**VS Code で Dev Container で開く**
- Command Palette（`Cmd+Shift+P` / `Ctrl+Shift+P`）
- 「Dev Containers: Reopen in Container」を選択
- 自動的に LaTeX 環境が構築されます

### GitHub Codespaces で開く（推奨：簡単）
- https://github.com/Kazusasakazusasa/Love_Common_test
- `Code` → `Codespaces` → `Create codespace on main`
- ブラウザで開発可能

---

## 👥 共同作業ガイド

### 初期設定
```bash
# リポジトリをクローン
git clone https://github.com/Kazusasakazusasa/Love_Common_test.git
cd Love_Common_test

# ユーザー情報を設定
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

### 作業の流れ

#### 1. 最新版に更新
```bash
git pull origin main
```

#### 2. 新しいブランチを作成
```bash
git checkout -b feature/機能名
# または
git checkout -b fix/バグ名
```

#### 3. ファイルを編集
LaTeX ファイルを編集します

#### 4. 変更をコミット
```bash
git add aQUIZZ.tex
git commit -m "Add: 新しい問題を追加" # わかりやすいメッセージを付ける
```

#### 5. プッシュして共有
```bash
git push origin feature/機能名
```

### Git コマンド一覧

| コマンド | 説明 |
|---------|------|
| `git status` | 変更ファイル一覧を表示 |
| `git diff` | 変更内容を確認 |
| `git log` | コミット履歴を表示 |
| `git pull` | リモートの最新版をダウンロード |
| `git push` | ローカルの変更をアップロード |

---

## ⚙️ 設定

### LaTeX ビルド設定
- **エンジン**: pLaTeX（日本語対応）
- **変換**: dvipdfmx（DVI → PDF）
- **自動ビルド**: ファイル保存時に自動実行

### 自動コミット
- **実行タイミング**: 10分ごと
- **内容**: 変更があれば自動的に GitHub にアップロード
- **メッセージ**: `Auto-commit: Update LaTeX files at [日時]`

### 無視ファイル（`.gitignore`）
以下は Git に追加されません：
- `*.pdf`, `*.aux`, `*.log` などの生成ファイル
- `.DS_Store`, `.vscode/` などの OS/IDE ファイル

---

## 📁 ファイル構成

```
Love_Common_test/
├── aQUIZZ.tex          # メインの LaTeX ファイル
├── aQUIZZ.pdf          # 生成される PDF（Git で管理しない）
├── memo                # 進捗メモ
├── TEST_quiz/          # テスト問題
├── README.md           # このファイル
└── .devcontainer/      # 開発環境設定
    ├── devcontainer.json
    └── Dockerfile
```

---

## 🐛 トラブルシューティング

### ビルドが失敗する
```bash
# キャッシュをクリア
rm *.aux *.log *.dvi *.pdf
```

### 変更がコンフリクトした
```bash
# 最新版をプル
git pull origin main

# コンフリクトを手動で解決後
git add .
git commit -m "Resolve conflict"
git push
```

---

## 📞 連絡

- Discordで大きな変更を事前に相談
- わからないことは質問してください！

---

**最後に更新**: 2026-06-16

