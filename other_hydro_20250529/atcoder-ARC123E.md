## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc123/tasks/arc123_e

$ X $ さんと $ Y $ さんの $ 2 $ 人のプログラマが、競技プログラミングを始めることになりました。

競技プログラミングの実力は、「レベル」と呼ばれる正の整数で表され、はじめ $ X $ さんのレベルは $ A_X $、$ Y $ さんのレベルは $ A_Y $ です。$ 2 $ 人はこれから練習メニューをこなすことで、レベルを上げていきます。

$ 2 $ 人のレベルの上がり方について、次のことが分かっています：

- $ X $ さんはちょうど $ B_X $ 個の練習メニューをこなすたびに、レベルがひとつ上がります。
- $ Y $ さんはちょうど $ B_Y $ 個の練習メニューをこなすたびに、レベルがひとつ上がります。

$ n\ =\ 1,\ 2,\ \ldots,\ N $ のうちで次を満たすものはいくつあるかを答えてください。

- $ 2 $ 人がちょうど $ n $ 個ずつの練習メニューをこなした場合、$ 2 $ 人の最終的なレベルは等しくなる。

一つの入力ファイルにつき、$ T $ 個のテストケースに答えてください。

## 输入格式
入力は以下の形式で標準入力から与えられます。

> $ T $ $ \text{case}_1 $ $ \text{case}_2 $ $ \vdots $ $ \text{case}_T $

各テストケースは以下の形式で与えられます。

> $ N $ $ A_X $ $ B_X $ $ A_Y $ $ B_Y $

## 输出格式
答えを出力してください。

## 题目大意
## 题目描述

两位程序员 $X$ 和 $Y$ 将开始一场编程竞赛。

一位程序员的编程技术可以用一个等级来表示。最初，$X$ 的等级是 $A_X$ ,$Y$ 的等级是 $B_Y$ 。两位程序员将通过任务学习提高自己的等级。

我们知道以下条件：

- $X$ 每学习 $B_X$ 个任务，就能提高 $1$ 个等级。
- $Y$ 每学习 $B_Y$ 个任务，就能提高 $1$ 个等级。

有多少个 $n$ 可以满足下列条件？

- $1 \le n \le N$ 。
- 学习 $n$ 个任务后， $X$ 和 $Y$ 的等级相等。

每一个输入文件中包含 $T$ 组数据 。

## 数据范围

- $1 \le T \le 2 \times 10^5$
- $1 \le N \le 10^9$
- $1 \le A_X,B_X,A_Y,B_Y \le 10^6$
- 所有输入都是整数。

Translated By [@joe_zxq](https://www.luogu.com.cn/user/623577) .

```input1
5
10 5 3 4 2
5 5 3 4 2
100 5 3 4 2
10 5 3 4 3
10 5 10 5 9
```

```output1
6
3
6
0
9
```

## 提示
### 制約

- $ 1\leq\ T\leq\ 2\times\ 10^5 $
- $ 1\leq\ N\leq\ 10^{9} $
- $ 1\leq\ A_X,\ B_X,\ A_Y,\ B_Y\ \leq\ 10^6 $

### Sample Explanation 1

ひとつめのテストケースについて説明します。 $ n\ =\ 1,\ 2,\ \ldots,\ 10 $ に対して、$ n $ 個の練習メニューをこなした場合の $ 2 $ 人のレベルは次のようになります： - $ X $ さんのレベル：$ 5,\ 5,\ 6,\ 6,\ 6,\ 7,\ 7,\ 7,\ 8,\ 8 $ - $ Y $ さんのレベル：$ 4,\ 5,\ 5,\ 6,\ 6,\ 7,\ 7,\ 8,\ 8,\ 9 $ $ 6 $ 個の $ n $ （$ n\ =\ 2,\ 4,\ 5,\ 6,\ 7,\ 9 $）の場合に $ 2 $ 人のレベルが等しくなります。したがって答えは $ 6 $ となります。

