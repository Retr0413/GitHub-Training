# GitHub ハンズオン研修（30分）

## 🎯 ゴール
GitHub未経験者が30分で実際の開発フローを体験し、基本操作を習得する

## 📝 今日やること
自分の自己紹介ファイル（README_名前.md）を作成し、チーム開発の流れを体験します

---

## 📋 事前準備
- GitHubアカウントの作成
- Git のインストール確認（`git --version`）
- 研修用リポジトリへのアクセス権限

---

## 🚀 ハンズオン手順

### Step 1: リポジトリをクローン（5分）
```bash
# リポジトリをローカルにコピー
git clone https://github.com/Retr0413/GitHub-Training.git
cd GitHub-Training
```

### Step 2: 作業ブランチを作成（3分）
```bash
# 自分の名前でブランチを作成
git checkout -b feature/add-readme-[あなたの名前]

# 例: git checkout -b feature/add-readme-tanaka
```

### Step 3: 自己紹介ファイルを作成（7分）
```bash
# ファイルを新規作成（名前は自分の名前に変更）
touch README_[あなたの名前].md
```

ファイルに以下の内容を記入：
```markdown
# 自己紹介 - [あなたの名前]

## 基本情報
- **名前**: [フルネーム]
- **所属**: [部署/チーム名]
- **入社年月**: [YYYY年MM月]

## 好きなこと・趣味
- [趣味1]
- [趣味2]

## GitHubを使ってやりたいこと
[今後GitHubでやってみたいことを1-2行で]
```

### Step 4: 変更をコミット（5分）
```bash
# 変更を確認
git status

# ファイルをステージング
git add README_[あなたの名前].md

# コミット（メッセージは分かりやすく）
git commit -m "Add: 自己紹介ファイルを追加 ([あなたの名前])"
```

### Step 5: リモートにプッシュ（3分）
```bash
# 作成したブランチをリモートに送信
git push origin feature/add-readme-[あなたの名前]
```

### Step 6: プルリクエスト（PR）を作成（5分）
1. ブラウザでGitHubリポジトリを開く
2. 「Compare & pull request」ボタンをクリック
3. PRタイトル: `自己紹介を追加: [あなたの名前]`
4. 本文に以下を記入：
   ```
   ## 変更内容
   - README_[名前].md を追加しました
   - 自己紹介を記載しました
   
   ## 確認事項
   - [ ] ファイル名が正しい
   - [ ] 内容が記入されている
   ```
5. 「Create pull request」をクリック

### Step 7: レビュー＆マージ（2分）
- 4年がPRを確認
- 問題なければマージ
- **おめでとうございます！** 🎉

---

## ✅ 成功の確認
- mainブランチに自分の README_名前.md が追加されている
- コントリビューターとして記録が残る

## 💡 学んだこと
- [ ] git clone - リポジトリの複製
- [ ] git checkout -b - ブランチ作成
- [ ] git add/commit - 変更の記録
- [ ] git push - リモートへの送信
- [ ] Pull Request - チーム開発の基本
