## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc132/tasks/abc132_a

長さ $ 4 $ の英大文字からなる文字列 $ S $ が与えられます。 $ S $ がちょうど $ 2 $ 種類の文字からなり、かつ現れる各文字はちょうど $ 2 $ 回ずつ現れているかどうかを判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
$ S $ がちょうど $ 2 $ 種類の文字からなり、かつ現れる各文字はちょうど $ 2 $ 回ずつ現れているなら `Yes` を、そうでないなら `No` を出力せよ。

## 题目大意
有长度为 $4$ 的由大写英文字母构成的串 $S$ ，问其是否恰好含有两种不同字母且这两种字母都恰好出现两次。

### 输入格式

$S$ 。

### 输出格式

如果符合要求输出`Yes`，否则输出`No`。

```input1
ASSA
```

```output1
Yes
```

```input2
STOP
```

```output2
No
```

```input3
FFEE
```

```output3
Yes
```

```input4
FREE
```

```output4
No
```

## 提示
### 制約

- $ S $ の長さは $ 4 $ である
- $ S $ は英大文字からなる

### Sample Explanation 1

$ S $ は `A` と `S` からなり、`A` と `S` はそれぞれ $ 2 $ 回ずつ現れます。

