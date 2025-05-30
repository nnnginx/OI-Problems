## 题目描述
[problemUrl]: https://atcoder.jp/contests/agc055/tasks/agc055_b

`A`, `B`, `C` からなる長さ $ N $ の文字列 $ S $ が与えられます。あなたは、次の操作を何回でも行うことができます。

- $ S_iS_{i+1}S_{i+2} $ が `ABC`, `BCA`, `CAB` のいずれかに等しいような $ 1\ \le\ i\ \le\ N-2 $ を任意に選ぶ。そして、その三文字を `ABC`, `BCA`, `CAB` のいずれかで置換する。

例えば、文字列 `AABC` に対して、以下の変換を行うことができます。

- `AABC` $ \to $ `ABCA` $ \to $ `BCAA`

上記の操作を有限回行うことで（$ 0 $ 回でもよい）、文字列 $ S $ から文字列 $ T $ を得ることが可能か判定してください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ T $

## 输出格式
上記の操作で $ S $ を $ T $ に変換することが可能であれば `YES`、そうでなければ `NO` と出力せよ。大文字、小文字は不問である。

## 题目大意
给定两个长度为 $n$ 的字符串 $a,b$。

你可以进行若干次以下操作：

- 若 $a$ 中的一个**子串**为 `ABC`，`BCA` 或 `CAB`，那么可以将这个子串替换为 `ABC`，`BCA` 或 `CAB`。

求能否将 $a$ 变成 $b$，输出 `YES` 或 `NO`。

```input1
4
AABC
BCAA
```

```output1
YES
```

```input2
4
ABCA
BCAB
```

```output2
NO
```

## 提示
### 制約

- $ 3\le\ N\ \le\ 5\cdot\ 10^5 $
- $ S $ は、`A`, `B`, `C` からなる長さ $ N $ の文字列である。
- $ T $ は、`A`, `B`, `C` からなる長さ $ N $ の文字列である。

### Sample Explanation 1

これは問題文で説明した例です。

