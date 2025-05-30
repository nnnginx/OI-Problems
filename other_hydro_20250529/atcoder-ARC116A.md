## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc116/tasks/arc116_a

正整数 $ N $ が与えられます。 $ N $ の正の奇数の約数と正の偶数の約数はどちらが多いか答えてください。

$ T $ 個のテストケースが与えられるので、それぞれについて答えを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ T $ $ case_1 $ $ \vdots $ $ case_T $

各ケースは以下の形式で与えられる。

> $ N $

## 输出格式
$ T $ 行出力せよ。 $ i $ 行目には $ case_i $ に対応する答えを出力せよ。各ケースでは、正の奇数の約数の方が多ければ `Odd` と、正の偶数の約数の方が多ければ `Even` と、同数であれば `Same` と出力せよ。

## 题目大意
一个正整数 $ N $ 。 求它约数的个数，若奇约数数量比偶约数多则输出  `Odd`  ，若偶约数数量比奇约数多则输出 `Even ` , 否则输出`Same`。

```input1
3
2
998244353
1000000000000000000
```

```output1
Same
Odd
Even
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ T\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ N\ \leq\ 10^{18} $

### Sample Explanation 1

$ 2 $ は $ 1 $ つの正の奇数の約数と、 $ 1 $ つの正の偶数の約数を持ちます。

