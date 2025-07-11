# AT_joi2022_yo2_a 図書館 2 (Library 2)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/joi2022yo2/tasks/joi2022_yo2_a

読書好きのビ太郎は図書館で本を借りて読むことにした．ビ太郎の家は狭いため，床には本 $ 1 $ 冊分の広さのスペースしかない．ただし高さは十分にあるため，ビ太郎はこのスペースに本を積んで管理することにした．

ビ太郎はこれから $ Q $ 回の行動を取る．$ i $ ($ 1\ \leqq\ i\ \leqq\ Q $) 回目の行動は文字列 $ S_i $ で表される．$ S_i $ は 英小文字からなる文字列か `READ` のいずれかであり，その意味は次の通りである．

- 英小文字からなる文字列の場合，ビ太郎は書名が $ S_i $ である本を図書館から借り，スペースの一番上に積む．
- `READ` の場合，ビ太郎はスペースの一番上に積まれている本を読み，図書館に返却する．

あなたはビ太郎がどの本をどのような順番で読んだのかを調べたい．

$ Q $ 回の行動の内容が与えられたとき，ビ太郎が読んだ本の書名を読んだ順に出力するプログラムを作成せよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ Q $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_Q $

## 输出格式

標準出力に，$ S_i $ が `READ` である行動のそれぞれに対して，ビ太郎が読んだ本の書名を順に改行区切りで出力せよ．

## 输入输出样例 #1

### 输入 #1

```
7
joi
joig
ioi
READ
egoi
READ
READ
```

### 输出 #1

```
ioi
egoi
joig
```

## 输入输出样例 #2

### 输入 #2

```
20
one
READ
two
three
four
five
six
seven
READ
eight
nine
READ
ten
eleven
READ
READ
twelve
READ
READ
READ
```

### 输出 #2

```
one
seven
nine
eleven
ten
twelve
eight
six
```

## 说明/提示

### 制約

- $ 2\ \leqq\ Q\ \leqq\ 200\,000 $．
- $ Q $ は整数である．
- $ S_i $ は長さ $ 1 $ 以上 $ 10 $ 以下の文字列である ($ 1\ \leqq\ i\ \leqq\ Q $)．
- $ S_i $ は英小文字からなる文字列または `READ` である ($ 1\ \leqq\ i\ \leqq\ Q $)．
- $ S_i $ が `READ` であるような $ i $ ($ 1\ \leqq\ i\ \leqq\ Q $) は $ 1 $ つ以上存在する．
- $ S_i $ が `READ` のとき，必ずスペースに $ 1 $ 冊以上の本が存在する ($ 1\ \leqq\ i\ \leqq\ Q $) ．

### 小課題

1. ($ 40 $ 点) $ Q\ \leqq\ 2\,000 $．
2. ($ 60 $ 点) 追加の制約はない．

### 採点に関する注意

すべての提出はジャッジシステム上で採点される．

提出されたソースコードは，小課題に対応するすべての採点用入力データについて正しい結果を返したとき，その小課題について正解と認められる．

各提出の得点は，提出されたソースコードについて正解と認められた小課題の得点の合計である．

この課題の得点は，**この課題に対するすべての提出の得点の最大値**である．

現在の得点は「提出結果」タブの「自分の得点状況」から確認できる．

### Sample Explanation 1

この入力例ではビ太郎は以下のように行動する． 1. 書名が `joi` である本をスペースに積む．このとき，スペースに積まれている本の書名は `joi` となる． 2. 書名が `joig` である本をスペースに積む．このとき，スペースに積まれている本の書名は上から順に `joig` ，`joi` となる． 3. 書名が `ioi` である本をスペースに積む．このとき，スペースに積まれている本の書名は上から順に `ioi` ，`joig` ，`joi` となる． 4. 書名が `ioi` である本を読んで返却する．このとき，スペースに積まれている本の書名は上から順に `joig` ，`joi` となる． 5. 書名が `egoi` である本をスペースに積む．このとき，スペースに積まれている本の書名は上から順に `egoi` ，`joig` ，`joi` となる． 6. 書名が `egoi` である本を読んで返却する．このとき，スペースに積まれている本の書名は上から順に `joig` ，`joi` となる． 7. 書名が `joig` である本を読んで返却する．このとき，スペースに積まれている本の書名は `joi` となる． よってビ太郎が読んだ本の書名 `ioi` ，`egoi` ，`joig` を順に改行区切りで出力する． この入力例はすべての小課題の制約を満たす．

### Sample Explanation 2

この入力例はすべての小課題の制約を満たす．