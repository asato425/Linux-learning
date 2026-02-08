# 第1章で学んだコマンド (Commands from Chapter 1)

第1章では主に概念的な内容のため、コマンドは少ないですが、
Linuxの基本的なコマンドをいくつか紹介します。

## システム情報の確認

### uname - システム情報の表示
```bash
# Linuxカーネルのバージョン確認
uname -r

# システムの詳細情報
uname -a
```

**実行例**:
```
$ uname -r
5.15.0-56-generic

$ uname -a
Linux hostname 5.15.0-56-generic #62-Ubuntu SMP x86_64 GNU/Linux
```

### whoami - 現在のユーザー名表示
```bash
whoami
```

**実行例**:
```
$ whoami
username
```

### date - 日付と時刻の表示
```bash
date
```

**実行例**:
```
$ date
Sat Feb  8 13:00:00 JST 2026
```

## その他の基本コマンド

### echo - メッセージの表示
```bash
echo "Hello, Linux!"
```

### man - マニュアルの表示
```bash
# コマンドのマニュアルを表示
man uname
```

## コマンド実行メモ
(実際に実行したコマンドとその結果をここに記録)
