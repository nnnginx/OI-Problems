## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc034/tasks/agc034_b

`A`,`B`,`C` からなる文字列 $ s $ が与えられます。

すぬけ君は $ s $ に対して次の操作をできるだけ多く行おうとしています。

- $ s $ の連続した部分文字列であって `ABC` であるようなものをひとつ選び、 `BCA` に書き換える。

操作回数の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式
操作回数の最大値を出力せよ。

## 题目大意
您将得到一个由 A，B 和 C 组成的字符串 s。

Snuke 希望在 s 上执行多次以下操作：

选择一个连续的 s 的子字符串，该字符串是 `ABC` 并将其替换为 `BCA`。

找到最大可能的操作数。

```input1
ABCABC
```

```output1
3
```

```input2
C
```

```output2
0
```

```input3
ABCACCBABCBCAABCB
```

```output3
6
```

## 提示
### 制約

- $ 1\ ≦\ |s|\ ≦\ 200000 $
- $ s $ の各文字は `A`,`B`,`C` のいずれか

### Sample Explanation 1

`ABCABC` → `BCAABC` → `BCABCA` → `BCBCAA` とすることで $ 3 $ 回操作可能で、これが最大です。

