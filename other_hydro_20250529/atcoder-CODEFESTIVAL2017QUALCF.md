## 题目描述
[problemUrl]: https://atcoder.jp/contests/code-festival-2017-qualc/tasks/code_festival_2017_qualc_f

$ 3 $ 人の男性 A, B, C が一緒に寿司を食べることになりました。 最初、$ N $ 種類の寿司が $ 1 $ 個ずつあります。 寿司には $ 1 $ から $ N $ まで番号が振られています。 ただし、$ N $ は $ 3 $ の倍数とします。

$ 3 $ 人はそれぞれ寿司に対して好き嫌いの順位付けを持っています。 A の順位付けは、$ 1 $ から $ N $ までの順列 $ (a_1,\ ...,\ a_N) $ で表されます。 各 $ i $ ($ 1\ \leq\ i\ \leq\ N $) について、A が $ i $ 番目に好きな寿司は寿司 $ a_i $ です。 同様に、B および C の順位付けは、$ 1 $ から $ N $ までの順列 $ (b_1,\ ...,\ b_N) $ および $ (c_1,\ ...,\ c_N) $ で表されます。

寿司がすべて無くなるか、喧嘩が起こる (後述) まで、$ 3 $ 人は次の行動を繰り返します。

- A, B, C はそれぞれ、残りの寿司のうち最も好きな寿司を見つける。 これらをそれぞれ寿司 $ x $, $ y $, $ z $ とする。 $ x $, $ y $, $ z $ がすべて相異なるならば、A, B, C はそれぞれ寿司 $ x $, $ y $, $ z $ を食べる。 そうでないならば、$ 3 $ 人は殴り合いの喧嘩を始める。

A および B の順位付け $ (a_1,\ ...,\ a_N) $ および $ (b_1,\ ...,\ b_N) $ が与えられます。 C の順位付け $ (c_1,\ ...,\ c_N) $ のうち、$ 3 $ 人が喧嘩を始めることなく寿司をすべて食べ切れるようなものは、何通りあるでしょうか？ $ 10^9+7 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ ... $ $ a_N $ $ b_1 $ $ ... $ $ b_N $

## 输出格式
C の順位付け $ (c_1,\ ...,\ c_N) $ のうち、$ 3 $ 人が喧嘩を始めることなく寿司をすべて食べ切れるようなものは、何通りあるか？ $ 10^9+7 $ で割った余りを出力せよ。

## 题目大意
有 $3$ 个长度为 $n$ 的排列，保证 $n$ 是 $3$ 的倍数。

对于一组三个排列，我们用下述算法判定其是否合法：维护一个初始为空的数组，每次从三个排列中各找到最前的未在上述数组中出现的数，之后把它们扔进上述数组。当且仅当某次处理过程中，三个排列给出的数有相同的，此时此排列组不合法。若直到上述数组中出现了 $1\sim n$ 所有数也没有出现上述情况，则此排列组合法。

给定前两个排列，求使排列组合法的第三个排列的数量。

```input1
3
1 2 3
2 3 1
```

```output1
2
```

```input2
3
1 2 3
1 2 3
```

```output2
0
```

```input3
6
1 2 3 4 5 6
2 1 4 3 6 5
```

```output3
80
```

```input4
6
1 2 3 4 5 6
6 5 4 3 2 1
```

```output4
160
```

```input5
9
4 5 6 7 8 9 1 2 3
7 8 9 1 2 3 4 5 6
```

```output5
33600
```

## 提示
### 制約

- $ 3\ \leq\ N\ \leq\ 399 $
- $ N $ は $ 3 $ の倍数である。
- $ (a_1,\ ...,\ a_N) $ および $ (b_1,\ ...,\ b_N) $ は $ 1 $ から $ N $ までの順列である。

### Sample Explanation 1

$ (c_1,\ c_2,\ c_3)\ =\ (3,\ 1,\ 2),\ (3,\ 2,\ 1) $ の $ 2 $ 通りです。 どちらの場合も、A, B, C はそれぞれ寿司 $ 1 $, $ 2 $, $ 3 $ を食べ、寿司がすべて無くなります。

### Sample Explanation 2

$ (c_1,\ c_2,\ c_3) $ がどのような順列であっても、A と B はともに寿司 $ 1 $ を食べようとするので、喧嘩が起こります。

### Sample Explanation 3

例えば $ (c_1,\ c_2,\ c_3,\ c_4,\ c_5,\ c_6)\ =\ (5,\ 1,\ 2,\ 6,\ 3,\ 4) $ の場合、まず A, B, C はそれぞれ寿司 $ 1 $, $ 2 $, $ 5 $ を食べ、次に A, B, C はそれぞれ寿司 $ 3 $, $ 4 $, $ 6 $ を食べ、寿司がすべて無くなります。

