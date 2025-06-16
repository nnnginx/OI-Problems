## 题目背景
本题数据极大，评测时可能需要较长时间等待。

## 题目描述
```plain
Byteasar intends to throw up a party.
```
Naturally, he would like it to be a success.  Furthermore, Byteasar is quite certain that to make it so it suffices if all invited guests  know each other.  He is currently trying to come up with a list of his friends he would like to invite.

Byteasar has $n$ friends, where $n$ is divisible by 3.

```plain
Fortunately, most of Byteasar's friends know one another.
```
Furthermore, Byteasar recalls that he once attended a party where there were $\frac{2}{3}n$ of his friends, and where everyone knew everyone else.

Unfortunately, Byteasar does not quite remember anything else from that    party.


In particular, he has no idea which of his friends attended it.

Byteasar does not feel obliged to throw a huge party, but he would like to    invite at least \frac{n}{3} of his friends.



He has no idea how to choose them, so he asks you for help.

## 输入格式
In the first line of the standard input two integers, $n$ and $m$ ($3\le n\le 3\ 000$, $\frac{\frac{2}{3}n(\frac{2}{3}n-1)}{2}\leq m\leq \frac{n(n-1)}{2}$), are given,separated by a single space.  These denote the number of Byteasar's friends and the number of pairs of his friends who know each other, respectively.

Byteasar's friends are numbered from 1 to $n$.

Each of the following $m$ lines holds two integers separated by a single      space.

The numbers in line no. $i+1$ (for $i=1,2,...,m$) are $a_i$ and $b_i$($1\le a_i<b_i\le n$), separated by a single space, which denote that the persons $a_i$ and $b_i$ know each other. Every pair of numbers appears at most once on the input.


## 输出格式
In the first and only line of the standard output your program should      print $\frac{n}{3}$ numbers, separated by single spaces, in increasing      order.  These number should specify the numbers of Byteasar's friends whom      he should invite to the party.  As there are multiple solutions, pick one      arbitrarily.


## 题目大意
### 题目描述

**译自 POI 2011 Round 3. Day 1. A「[Party](https://szkopul.edu.pl/problemset/problem/PCtteC6gKwc2ZikW8nUZzfyh/site/?key=statement)」**

Byteasar 打算举行一次聚会。他自然想要这次聚会成功进行。此外，Byteasar 确信只要邀请的嘉宾都互相认识就可以了。他目前在试着写一份邀请名单。

Byteasar 有 $n$ 个朋友，这里 $n$ 可以被 $3$ 整除。幸运的是，Byteasar 的朋友大部分都互相认识。并且 Byteasar 想起了一次他参加的聚会，那次聚会有 $ \frac{2}{3}n $ 个他的朋友参加，并且他们都互相认识。不幸的是，关于那次聚会的具体细节他不记得了……总的来说，他忘了是他的哪些朋友参加了。

Byteasar 认为他没有义务举办一个大型聚会，但他想邀请至少 $ \frac{n}{3} $ 个他的朋友。他不知道邀请谁，所以请你帮他。

### 输入格式

输入的第一行包含两个整数 $n,m$，表示 Byteasar 的朋友数和互相认识的朋友对数；

接下来 $m$ 行，每行两个整数 $a_i,b_i$， 表示朋友 $a_i,b_i$ 互相认识。每一对数最多在输入中出现一次。

### 输出格式

按编号升序，输出一行 $ \frac{n}{3} $ 个数，表示 Byteasar 要邀请的朋友编号。如果有多组解，输出任意一组均可。

### 样例解释

![](https://cdn.luogu.com.cn/upload/image_hosting/yjpf686v.png)

编号为 $1,3,4,5$ 的朋友互相认识。然而对于任意一对互相认识的朋友，如 $2,4$，都可以作为正确答案。即，这一对朋友并不一定来自于之前提到的那个四元组。

### 数据范围

对于全部数据，$ 3 \le n \le 3000 , \frac{\frac{2}{3}n(\frac{2}{3}n-1)}{2} \le m \le \frac{n(n-1)}{2}, 1 \le a_i \lt b_i \le n $。

翻译来自于 [LibreOJ](https://loj.ac/p/2166)。

```input1
6 10
2 5
1 4
1 5
2 4
1 3
4 5
4 6
3 5
3 4
3 6
```

```output1
2 4
```

