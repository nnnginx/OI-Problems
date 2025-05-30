## 题目描述
Xavier, a 9-year-old student, loves playing many kinds of puzzles. One of his favourites is the following:

Xerier, his classmate, has made many cards. She writes down a single positive number on each of them. No numbers written on different cards are the same. After that she writes down an equation, whose right side is a single positive number chosen by her, and the left side is the sum of $p$ integers:

Then she asks Xavier put $p$ cards on the corresponding $X_i$’s position to make this equation correct, with an additional condition that $X_i$ should be ordered from smaller to bigger, i.e.

Every time Xavier immediately comes up with many solutions. Now he wants to know how many solutions in total are there for any $n$ given by Xerier.

## 输入格式
There are multiple test cases. The number of them is given in the beginning of the input. Then a series of input block comes one by one.
 
For each test case:

The first line contains two space-separated integers $m$ and $p (1\leq p\leq 5)$. The second line contains $m$ distinct positive integers - the numbers written on each of the cards. None of these integers exceeds $13000$.

There are about $120$ test cases in total, but $90\%$ of them are relatively small. More precisely, all numbers are less than or equal to $100$ in $90\%$ of the test cases.

## 输出格式
For each test case:

For each positive integer, output the number of ways in a single line. To keep the output finite, only numbers with positive ways should be outputted.

Output a blank line after each test case. See sample for more format details.

## 题目大意
集合 $S$ 内有 $m$ 个互异整数。请对于任意整数 $i$ 求出 $S$ 内满足大小为 $p$ 且元素和为 $i$ 的子集数量。

输入格式：$T$ 组测试数据。对于每组数据，第一行输入整数 $m,p$，第二行输入 $m$ 个整数，表示 $S$ 内的元素。

输出格式：只需输出答案不为 $0$ 的 $i$ 及其对应的答案。每组测试数据之间以换行隔开。

```input1
3
3 3
1 2 3
5 4
1 3 5 6 7
10 3
1 2 3 4 5 6 7 8 9 10
```

```output1
Case #1:
6: 1

Case #2:
15: 1
16: 1
17: 1
19: 1
21: 1

Case #3:
6: 1
7: 1
8: 2
9: 3
10: 4
11: 5
12: 7
13: 8
14: 9
15: 10
16: 10
17: 10
18: 10
19: 9
20: 8
21: 7
22: 5
23: 4
24: 3
25: 2
26: 1
27: 1
```

