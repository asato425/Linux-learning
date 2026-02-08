# 学習の始め方 (Getting Started Guide)

このガイドでは、このリポジトリを使ってLinux標準教科書を効果的に学習する方法を説明します。

## 準備

1. Linux標準教科書を入手する
   - LPI-Japan公式サイトからダウンロード: https://linuc.org/textbooks/linux/
   
2. Linux環境を用意する
   - 実機にLinuxをインストール
   - VirtualBoxなどで仮想マシンを構築
   - WSL2 (Windows Subsystem for Linux)を利用
   - クラウド環境 (AWS, GCP, Azureなど)を利用

## 学習の進め方

### ステップ1: 章を読む
各章の内容を教科書で学習します。

### ステップ2: ノートを作成
`chapters/chapterXX/` ディレクトリに学習内容をまとめます：

1. `README.md` - 章の概要と学習目標を記入
2. `notes.md` - 詳細な学習ノートを作成
3. `commands.md` - 学んだコマンドをまとめる

### ステップ3: コマンドを実行
教科書に出てくるコマンドを実際に実行して、結果を記録します。

```bash
# 例：第2章のディレクトリを作成
cd chapters/
mkdir chapter02
cd chapter02
```

### ステップ4: 演習問題に取り組む
`exercises/chapterXX/` で演習問題を解きます：

1. `problems.md` に問題を記録
2. 自分で考えて解答
3. `solutions.md` に解答を記録
4. 実際にコマンドを実行して確認

### ステップ5: コマンドリファレンスを作成
`commands/` ディレクトリに、重要なコマンドのリファレンスを作成します。

## 記録のコツ

### コマンド実行結果の記録
```markdown
### ls コマンドの実行例
\`\`\`bash
$ ls -la
total 24
drwxr-xr-x  4 user user 4096 Feb  8 12:00 .
drwxr-xr-x 10 user user 4096 Feb  8 11:00 ..
-rw-r--r--  1 user user  220 Feb  8 12:00 .bashrc
\`\`\`
```

### エラーの記録も重要
エラーが発生した場合も、その内容と解決方法を記録しましょう。

```markdown
### エラー例
\`\`\`bash
$ cd /root
bash: cd: /root: Permission denied
\`\`\`

**原因**: rootディレクトリは一般ユーザーではアクセスできない  
**解決**: `sudo`を使うか、アクセス可能なディレクトリを使用
```

### 疑問点の記録
わからないことや疑問に思ったことも記録しておきましょう。

```markdown
## 疑問点
- なぜ`ls -l`と`ll`は同じ結果になるのか？
  → `ll`は`ls -l`のエイリアスとして設定されていることが多い
```

## おすすめの学習ペース

- 1章あたり: 1〜2週間
- 毎日の学習時間: 30分〜1時間
- 週末に復習: 1〜2時間

無理せず、自分のペースで学習を進めましょう。

## 学習を継続するために

1. **定期的に記録**: 学んだことはすぐに記録する習慣をつける
2. **実践重視**: コマンドは必ず自分で実行する
3. **復習**: 定期的に過去の章を見直す
4. **疑問を残さない**: わからないことは調べて解決する

## サンプルワークフロー

```bash
# 1. 新しい章のディレクトリを作成
cd /path/to/Linux-learning
mkdir -p chapters/chapter03
cd chapters/chapter03

# 2. テンプレートファイルを作成
touch README.md notes.md commands.md
mkdir examples

# 3. 学習しながらノートを作成
vim notes.md

# 4. コマンドを実行してログを記録
cd examples/
# ここで実際にコマンドを実行

# 5. 変更をコミット（ローカルで管理する場合）
cd /path/to/Linux-learning
git add .
git commit -m "第3章の学習ノートを追加"
```

## 参考リソース

- **Linux標準教科書**: https://linuc.org/textbooks/linux/
- **man コマンド**: コマンドのマニュアルを参照 (`man ls`)
- **tldr**: コマンドの簡易リファレンス (https://tldr.sh/)
- **Linux Journey**: https://linuxjourney.com/

頑張って学習を進めていきましょう！
