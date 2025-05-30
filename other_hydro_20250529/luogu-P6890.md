## 题目描述
Webmaster Kirk is reorganizing his school's website. There are a number of pages on the website and the
content is fine, but he noticed that the pages are not properly linked. In fact, every page contains exactly one link, pointing to some other page in the website. This is a poor design – starting from the homepage, a visitor will usually have to follow many links before reaching the page of his interest, and some pages might not be reachable from the homepage at all. As a first step, he wants to add a few links so that every page can be quickly accessed from the homepage. New links can be added anywhere in the website.

The website contains N pages marked with integers 1 to N and the homepage is marked with the number 1.

There are also N links; **each page contains exactly one link** pointing to some **different** page. For an integer
K, a website is said to be **K-reachable** if every page on the website other than the homepage can be reached from the homepage by following **at most K** links.

Write a program that, given the description of the website and an integer K, finds the **minimum number of links that need to be added** in order to make the website K-reachable.

## 输入格式
第一行是两个整数用空格隔开 $N$ 和 $K$。

接下来 $N$ 行：

其中第 $i+1$ 行 $(1\leqslant i\leqslant N)$ 输入两个整数 $x$ 和 $y$ , 表示存在一条从 $x$ 到 $y$ 的单向边。

## 输出格式
输出仅一个整数：表示最少需要添加的边数。

## 题目大意
给定一个 $N$ 个点 $N$ 条边的有向图（内向基环树）， 要求在图上添加最少的边，使得点 $1$ 到达所有其他点的最短路长度不超过 $K$。

```input1
8 3
1 2
2 3
3 5
4 5
5 6
6 7
7 8
8 5
```

```output1
2
```

```input2
14 4
1 2
2 3
3 4
4 5
7 5
5 6
6 3
8 10
10 9
9 8
14 13
13 12
12 11
11 14
```

```output2
3
```

## 提示
在第二组样例中，一个合法的路径集合 $\{1\to 7,1\to 14,14\to 10\}$。

$2 ≤ N ≤ 500 000$, $1 ≤ K ≤ 20 000$。

