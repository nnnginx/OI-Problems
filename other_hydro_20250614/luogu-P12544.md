## 题目描述
There are $n$ types of boys and $2 \cdot n$ girls. The types of boys are numbered with integers from $1$ to $n$, while the girls are numbered with integers from $1$ to $2 \cdot n$.

There are $c_i$ boys of the $i$-th type, and each of them likes girls numbered $a_i$ and $b_i$.

Find the size of the largest set of boys such that for every pair of boys in this set, there is at least one girl that both of them like.

In this problem, each test contains several sets of input data. You need to solve the problem independently for each such set.

## 输入格式
The first line contains one integer $T$ $(1 \le T \le 500)$ --- the number of sets of input data. The description of the input data sets follows.

In the first line of each input data set, there is one integer $n$ $(1 \le n \le 7 \cdot 10^5)$.

In the next $n$ lines, there are three integers $a_i$, $b_i$, $c_i$ $(1 \le a_i < b_i \le 2 \cdot n, 1 \le c_i \le 10^9)$ --- the parameters for the corresponding type of boys.

It is guaranteed that $a_i \ne a_j$ or $b_i \ne b_j$ for any $1 \le i < j \le n$.

It is guaranteed that the sum of $n$ across all input data sets of a single test does not exceed $7 \cdot 10^5$.

## 输出格式
For each set of input data, output one integer on a separate line --- the size of the largest set of boys such that for every pair of boys in this set, there is at least one girl that both of them like.

```input1
3
2
1 2 3
3 4 5
5
1 2 1
1 3 4
4 5 2
3 4 2
1 4 3
4
1 2 3
2 3 4
3 5 4
1 3 2
```

```output1
5
9
10
```

## 提示
Let $S$ be the sum of $n$ over all test case input sets of one test, and $K$ be the sum of all $c_i$ over all test case input sets of one test.

- ($5$ points): $n \le 5$;
- ($11$ points): $S \le 100$;
- ($7$ points): each girl is liked by boys of no more than two types;
- ($10$ points): $S \le 3000$;
- ($23$ points): $S \le 3 \cdot 10^5$;
- ($19$ points): $K \le 10^7$;
- ($25$ points): with no additional constraints.

