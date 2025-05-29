## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc118/tasks/arc118_d

素数 $ P $ および正の整数 $ a,\ b $ が与えられます。 $ P $ 項からなる整数列 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_P) $ であって、次の条件をすべて満たすものが存在するかを判定してください。 存在する場合には、そのようなものをひとつ出力してください。

- $ 1\leq\ A_i\leq\ P\ -\ 1 $
- $ A_1\ =\ A_P\ =\ 1 $
- $ (A_1,\ A_2,\ \ldots,\ A_{P-1}) $ は、$ (1,\ 2,\ \ldots,\ P-1) $ を並べ替えたものである
- 任意の $ 2\leq\ i\leq\ P $ に対して、次のうち少なくともひとつが成り立つ：
  - $ A_{i}\ \equiv\ aA_{i-1}\pmod{P} $
  - $ A_{i-1}\ \equiv\ aA_{i}\pmod{P} $
  - $ A_{i}\ \equiv\ bA_{i-1}\pmod{P} $
  - $ A_{i-1}\ \equiv\ bA_{i}\pmod{P} $

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ P $ $ a $ $ b $

## 输出格式
問題の条件を満たす整数列 $ A $ が存在するならば `Yes` を、そうでなければ `No` を出力してください。 `Yes` の場合には、$ 2 $ 行目にそのような整数列 $ A $ の各要素を、空白で区切って 1 行で出力してください。

> $ A_1 $ $ A_2 $ $ \ldots $ $ A_P $

条件を満たす整数列が複数存在する場合は、どれを出力しても正解となります。

## 题目大意
给定质数 $P$ 和两个正整数 $a,b$，要求构造一个长度为 $P$ 的序列满足：
- $1\le A_i\le P-1$；
- $A_1=A_P=1$；
- $(A_1,A_2,\dots,A_{P-1})$ 是一个 $1\sim P-1$ 的排列；
- $\forall 2\le i\le P$，满足下列四个条件中的至少一个：
	1. $A_i\equiv aA_{i-1}\pmod P$；
    2. $A_{i-1}\equiv aA_i\pmod P$；
    3. $A_i\equiv bA_{i-1}\pmod P$；
    4. $A_{i-1}\equiv bA_i\pmod P$。

$\texttt{Data Range}:2\le P\le 10^5,1\le a,b\le P-1$，$P$ 为质数。

Translated by pitham（脾土蛤蟆）。

```input1
13 4 5
```

```output1
Yes
1 5 11 3 12 9 7 4 6 8 2 10 1
```

```input2
13 1 2
```

```output2
Yes
1 2 4 8 3 6 12 11 9 5 10 7 1
```

```input3
13 9 3
```

```output3
No
```

```input4
13 1 1
```

```output4
No
```

## 提示
### 制約

- $ 2\leq\ P\leq\ 10^5 $
- $ P $ は素数
- $ 1\leq\ a,\ b\ \leq\ P\ -\ 1 $

### Sample Explanation 1

$ P\ =\ 13 $ を法として、 - $ A_2\equiv\ 5A_1 $ - $ A_2\equiv\ 4A_3 $ - $ \vdots $ - $ A_{13}\equiv\ 4A_{12} $ が成り立ち、この整数列は条件を満たすことが確認できます。

