## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc279/tasks/abc279_a

`v` と `w` のみからなる文字列 $ S $ が与えられます。

$ S $ の中に、下に尖っている部分が何箇所あるかを出力してください（入出力例にある図もご参照ください）。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式
答えを整数として出力せよ。

## 题目大意
有一个仅包含 `w` 和 `v` 的字符串 $S$，其中一个 `w` 加两分，一个 `v` 加一分。请输出该字符串的分数。

$1\le S$ 的长度 $\le 100$。

翻译提供：xiaohaoaibiancheng66

```input1
vvwvw
```

```output1
7
```

```input2
v
```

```output2
1
```

```input3
wwwvvvvvv
```

```output3
12
```

## 提示
### 制約

- $ S $ は `v` と `w` のみからなる文字列
- $ S $ の長さは $ 1 $ 以上 $ 100 $ 以下
 
### Sample Explanation 1

!\[vvwvw\](https://img.atcoder.jp/abc279/53a8734c956ed9751e1d02505ba8655c.png) 上の画像のように、`vvwvw` という文字列には下に尖った部分が $ 7 $ 箇所あります。

