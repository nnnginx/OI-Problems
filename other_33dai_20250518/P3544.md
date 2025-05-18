## 题目描述
A map of Mafiatown's road network is given.

The network consists of intersections and bidirectional streets that connect them.

The streets cross only at the intersections, but they may lead through tunnels or flyovers.

Each pair of intersections is linked by at most one street.

At every intersection $v$ there is a police station manned by $p(v)$ policemen.

A street linking the intersections $u$ and $v$ is considered safe if there are at least $b(u,v)$ policemen in total in the two stations at the streets ends. Initially    $p(u)+p(v)\ge b(u,v)$ holds for every street.

However, due to an ongoing crisis the mayor Byteasar has ordained the Minimalist Security Act (MSA), which states that:

a certain number (which may be zero) of policemen is to be laid off from each police station        (we denote the number of policemen laid off from the station at the intersection $v$ by $z(v)$),                  after the layoff, the total number of the policemen at both ends of every street connecting some two intersections,        say $u$ and $v$, should equal $b(u,v)$ exactly, i.e.:

$p(u)-z(u)+p(v)-z(v)=b(u,v)$ These rules do not determine uniquely how many policemen are to be laid off.

Byteasar wonders what is the minimum and the maximum number of laid off policemen    (the sum of $z$ values over all intersections) that complies with aforementioned rules.

## 输入格式
In the first line of the standard input there are two integers, $n$ and $m$ ($1\le n\le 500\ 000$, $0\le m\le 3\ 000\ 000$), separated by a single space, that denote    the number of intersections and the number of streets in Mafiatown, respectively.

The intersections are numbered from 1 to $n$.

In the second line $n$ nonnegative integers separated by single spaces are given.

These are the numbers of policemen currently employed at successive stations, i.e., the values $p(1),p(2),\cdots,p(n)$($0\le p(i)\le 10^6$).

Each of the following $m$ lines describes a single bidirectional street. Such description consists of three integers,$u_i,v_i,b(u_i,v_i)$($1\le u_i,v_i\le n$,$u_i\ne v_i$,$0\le b(u_i,v_i)\le 10^6$), separated by single spaces, that denote respectively: the numbers of the intersections at the ends of the street and the minimum total number of policemen that have to man the stations at those intersections.


## 输出格式
If Byteasar's ordinance can be carried out, your program should print, on the standard output,    exactly one line with two integers separated by a single space.

The numbers should be the minimum and the maximum number of policemen that should be laid off    in order to carry out the ordinance.

If carrying out the ordinance is impossible, your program should print a single line containing    the word NIE (Polish for no).


## 题目大意
### 题目描述

**译自 POI 2012 Stage 3. Day 2「[Bezpieczeństwo minimalistyczne](https://szkopul.edu.pl/problemset/problem/aSbIC_LB4H-CGMYPEVue5jFw/site/?key=statement)」**

给定一张无向图，点有点权 $p(v)$，边有边权 $b(u,v)$，初始时保证对每条边有 $p(u) + p(v) \ge b(u,v)$。

现在需要减少一部分点的点权，使得对每条边都恰有 $p(u) + p(v) = b(u,v)$.

求整张图减少的点权和的最小值和最大值。

### 输入格式

第一行两个整数 $n$ 和 $m$（$1 \le n \le 500\ 000,0 \le m \le 3\ 000\ 000$），表示图的点数和边数。

接下来一行 $n$ 个非负整数 $p(1),p(2),\ldots,p(n) (0 \le p(i) \le 10^6)$，表示点权。

接下来 $m$ 行每行三个整数 $u_i, v_i, b(u_i, v_i)$（$1 \le u_i,v_i \le n,u_i \neq v_i,0 \le b(u_i,v_i) \le 10^6$），表示边和边权。

### 输出格式

如果存在符合条件的方案，输出一行两个整数，表示整张图减少的点权和的最小值和最大值。

如果不存在，输出 `NIE`.

### 数据范围

对于 $56\%$ 的数据有 $n \le 2000,m \le 8000$.

对于所有数据有 $1 \le n \le 500\ 000,0 \le m \le 3\ 000\ 000$.

翻译来自于 [LibreOJ](https://loj.ac/p/2702)。

```input1
3 2
5 10 5
1 2 5
2 3 3
```

```output1
12 15
```

