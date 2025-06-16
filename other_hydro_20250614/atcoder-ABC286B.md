## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc286/tasks/abc286_b

長さ $ N $ の文字列 $ S $ が与えられます。

$ S $ に連続して含まれる `na` を全て `nya` に置き換えて得られる文字列を答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式
答えを出力せよ。

## 题目大意
给定一个长度为 $n$ 的只包含小写字母的字符串 $s$，我们对 $s$ 进行如下操作：

- 对于 $s$ 的每一个子串 `na`，将 `na` 变为 `nya`。

求操作完毕后的结果。

保证 $1 \le n \le 1000$。

翻译提供者：@\_\_Allen\_123\_\_

```input1
4
naan
```

```output1
nyaan
```

```input2
4
near
```

```output2
near
```

```input3
8
national
```

```output3
nyationyal
```

## 提示
### 制約

- $ N $ は $ 1 $ 以上 $ 1000 $ 以下の整数
- $ S $ は英小文字からなる長さ $ N $ の文字列
 
### Sample Explanation 1

`naan` に連続して含まれる `na` を全て `nya` に置き換えて得られる文字列は `nyaan` です。

### Sample Explanation 2

$ S $ に `na` が連続して含まれないこともあります。

