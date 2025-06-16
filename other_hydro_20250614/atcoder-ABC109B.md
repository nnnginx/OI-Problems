## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc109/tasks/abc109_b

高橋くんは今日も $ 1 $ 人でしりとりの練習をしています。

しりとりとは以下のルールで遊ばれるゲームです。

- はじめ、好きな単語を発言する
- 以降、次の条件を満たす単語を発言することを繰り返す
  - その単語はまだ発言していない単語である
  - その単語の先頭の文字は直前に発言した単語の末尾の文字と一致する

高橋くんは、$ 10 $ 秒間にできるだけ多くの単語を発言する練習をしています。

高橋くんが発言した単語の個数 $ N $ と $ i $ 番目に発言した単語 $ W_i $ が与えられるので、どの発言もしりとりのルールを守っていたかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ W_1 $ $ W_2 $ $ : $ $ W_N $

## 输出格式
高橋くんのどの発言もしりとりのルールを守っていたなら `Yes`、そうでなければ `No` を出力せよ。

## 题目大意
有 $n$ 个字符串，需要同时满足第 $i$ 个字符串没有出现过和第 $i$ 个字符串的首字母必须是第 $i - 1$ 个字符串的最后一个字母。只要不满足其中任意一个要求就输出"No"，否则输出"Yes"。

```input1
4
hoge
english
hoge
enigma
```

```output1
No
```

```input2
9
basic
c
cpp
php
python
nadesico
ocaml
lua
assembly
```

```output2
Yes
```

```input3
8
a
aa
aaa
aaaa
aaaaa
aaaaaa
aaa
aaaaaaa
```

```output3
No
```

```input4
3
abc
arc
agc
```

```output4
No
```

## 提示
### 制約

- $ N $ は $ 2\ \leq\ N\ \leq\ 100 $ を満たす整数である
- $ W_i $ は英小文字からなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列である

### Sample Explanation 1

`hoge` が複数回発言されているのでしりとりのルールを守っていません。

