# AT_abc276_f [ABC276F] Double Chance

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc276/tasks/abc276_f

カード $ 1 $, カード $ 2 $, $ \ldots $, カード $ N $ の $ N $ 枚のカードがあり、 カード $ i $ $ (1\leq\ i\leq\ N) $ には整数 $ A_i $ が書かれています。

$ K=1,2,\ldots,N $ について、次の問題を解いてください。

> カード $ 1 $, カード $ 2 $, $ \ldots $, カード $ K $ の $ K $ 枚のカードが入っている袋があります。  
> 次の操作を $ 2 $ 回繰り返し、記録された数を順に $ x,y $ とします。
> 
> > 袋から無作為にカードを $ 1 $ 枚取り出し、カードに書かれている数を記録する。その後、カードを **袋の中に戻す** 。
> 
> $ \max(x,y) $ の値の期待値を $ \text{mod}\ 998244353 $ で出力してください（注記参照）。  
> ただし、$ \max(x,y) $ で $ x $ と $ y $ のうち小さくない方の値を表します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

$ N $ 行出力せよ。 $ i $ 行目 $ (1\leq\ i\leq\ N) $ には、$ K=i $ の時の問題に対する答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
5 7 5
```

### 输出 #1

```
5
499122183
443664163
```

## 输入输出样例 #2

### 输入 #2

```
7
22 75 26 45 72 81 47
```

### 输出 #2

```
22
249561150
110916092
873463862
279508479
360477194
529680742
```

## 说明/提示

### 注記

求める期待値は必ず有限値かつ有理数となることが証明できます。また、この問題の制約下では、その値を互いに素な $ 2 $ つの整数 $ P $, $ Q $ を用いて $ \frac{P}{Q} $ と表したとき、$ R\ \times\ Q\ \equiv\ P\pmod{998244353} $ かつ $ 0\ \leq\ R\ \lt\ 998244353 $ を満たす整数 $ R $ がただ一つ存在することが証明できます。この $ R $ を出力してください。

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 2\times\ 10^5 $
- 入力は全て整数

### Sample Explanation 1

例えば、$ K=2 $ の時の答えは次のようにして求まります。 袋の中にはカード $ 1 $ とカード $ 2 $ が入っており、それぞれには $ A_1=5 $ と $ A_2=7 $ が書かれています。 - $ 1 $ 回目に取り出されたカードがカード $ 1 $ 、$ 2 $ 回目に取り出されたカードもカード $ 1 $ のとき、$ x=y=5 $ であり、$ \max(x,y)=5 $ となります。 - $ 1 $ 回目に取り出されたカードがカード $ 1 $ 、$ 2 $ 回目に取り出されたカードはカード $ 2 $ のとき、$ x=5 $, $ y=7 $ であり、$ \max(x,y)=7 $ となります。 - $ 1 $ 回目に取り出されたカードがカード $ 2 $ 、$ 2 $ 回目に取り出されたカードはカード $ 1 $ のとき、$ x=7 $, $ y=5 $ であり、$ \max(x,y)=7 $ となります。 - $ 1 $ 回目に取り出されたカードがカード $ 2 $ 、$ 2 $ 回目に取り出されたカードもカード $ 2 $ のとき、$ x=y=7 $ であり、$ \max(x,y)=7 $ となります。 これらが等確率で起こるため、期待値は $ \frac{5+7+7+7}{4}=\frac{13}{2} $ となります。 $ 499122183\times\ 2\equiv\ 13\ \pmod{998244353} $ であるため、$ 499122183 $ を出力します。