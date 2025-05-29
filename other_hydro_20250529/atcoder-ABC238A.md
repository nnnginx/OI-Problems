## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc238/tasks/abc238_a

$ 2^n\ \gt\ n^2 $ ですか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ n $

## 输出格式
$ 2^n\ \gt\ n^2 $ なら `Yes` を、そうでないなら `No` を出力せよ。

## 题目大意
给定一个小于 $10^9$ 的正整数 $n$，问 $2^n$ 和 $n^2$ 那个更大？

```input1
5
```

```output1
Yes
```

```input2
2
```

```output2
No
```

```input3
623947744
```

```output3
Yes
```

## 提示
### 制約

- $ n $ は $ 1 $ 以上 $ 10^9 $ 以下の整数

### Sample Explanation 1

$ 2^5=32,\ 5^2=25 $ より $ 2^n\ \gt\ n^2 $ であるため、`Yes` を出力します。

### Sample Explanation 2

$ n=2 $ の場合 $ 2^n=n^2=2^2 $ となり、故に $ 2^n\ \gt\ n^2 $ ではありません。よって `No` を出力します。

