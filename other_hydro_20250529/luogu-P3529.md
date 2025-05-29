## 题目描述
Bartie and his friends compete in the Team Programming Contest.

There are $n$ contestants on each team, and each team has access to $n$ computers.

The contest lasts $t$ minutes, during which the contestants are to solve $m$ programming problems.

Furthermore, penalties are imposed on the teams: solving a problem $s$ minutes since the beginning of the contest amounts to $s$ penal points.

The team that solved the most problems wins the contest, with ties broken in    favour of the team with smaller penalty.

On the contest day Bartie quickly glances over the problem statements and    distributes them among his teammates.

He knows his team so well that he can exactly assess who is able to solve    which problem.

Solving any problem takes any contestant that is able to solve it exactly $r$ minutes of using the computer.

Bartie's team did not fare well in this year's contest.

Bartie is obsessed with the thought that it might be his fault, due to wrong    decisions regarding the distribution of problems.

He asks you to write a program that, given what Bartie knew at the beginning    of the contest, determines the best possible result of Bytie's team, together    with the assignment of problems to team members that attains the result.


## 输入格式
Five integers $n$, $m$, $r$, $t$, and $k$ ($1\le n,m\le 500$, $1\le r,t\le 1\ 000\ 000$) are given in the first line of the standard input, separated by single spaces.

These denote, respectively:

the number of contestants on a team, the number of problems, the time it      takes a contestant to solve a problem, the duration of the contest,and the number of contestant-problem pairs given on the input.

Each of the following $k$ lines holds two integers $a$ and $b$($1\le a\le n$,$1\le b\le m$), separated by a single space, denoting that the contestant $a$ is able to solve the problem $b$.Each such pair appears at most once in the input.

In tests worth at least 30% of the points it additionally holds that $n,m\le 100$.


## 输出格式
In the first line of the standard output the best possible result of Bytie's      team should be printed as two numbers separated by a single space:

the number of solved problems $z$ and the total penal points.

An exemplary assignment of problems that attains this result should be given in the following $z$ lines.

Each of those should hold three integers $a$, $b$ and $c$ ($1\le a\le n$,$1\le b\le m$, $0\le c\le t-r$),separated by single spaces, signifying that the contestant $a$ should start solving the problem $b$ at time $c$(the contest starts at time $0$).No contestant should be assigned a problem that they cannot solve. If more that one optimal assignment exists, your program can output any of them.


## 题目大意
### 题目描述
**译自 POI 2011 Round 3. Day 2. C「[Programming Contest](https://szkopul.edu.pl/problemset/problem/VwDLJhYqi1z_sZrb2NyfvQ5e/site/?key=statement)」**

Bartie 和他的朋友们都在打团体程序设计竞赛。每个队有 $n$ 名队员，每个队可以用 $n$ 台电脑。比赛持续 $t$ 分钟，比赛中选手们要解决 $m$ 道程序设计题目。此外，比赛会按如下规则记罚时：比赛开始 $s$ 分钟通过了一道题，则罚时加 $s$ 分。解题数目最多的队伍获胜，如果解题数目相同，罚时最少的队伍获胜。

在一次比赛中，Bartie 迅速浏览了全部题目并且把题目分配给了队友。他十分了解队友，并可以把题目分配给能解决这道题的人。对于每个选手，解决一道题的时间都恰好是 $r$ 分钟。

Bartie 的队伍在今年的比赛中表现不佳。Bartie 确信这是他的问题，是由于他分配问题失误造成的。他想让你写个程序，给出 Bartie 在比赛前知道的信息，请求出 Bartie 的队伍可能的最好成绩和分配题目的方式。

### 输入格式

第一行五个整数 $n,m,r,t,k$，分别表示一个队中的队员数，题目数，队员解决一道题的用时，比赛的时间长度和队员-题目对数；

接下来 $k$ 行，每行两个数 $a,b$，表示队员 $a$ 可以解决问题 $b$。每一个有序对在输入中最多出现一次。

### 输出格式

第一行输出两个整数，用一个空格隔开，分别表示解出的题目总数 $z$ 和最少总罚时。

接下来 $z$ 行，每行输出三个整数 $a,b,c\ (1 \le a \le n , 1 \le b \le m , 0 \le c \le t-r)$，表示队员 $a$ 在时刻 $c$ 时开始解决题目 $b$（比赛开始于时刻 $0$）。你不能把一道题分配给不会解决它的人。如果有多种分配方案，输出任意一组均可。

### 数据范围

对于全部数据，$ 1 \le n, m \le 500 , 1 \le r, t \le 1000000, 1 \le a \le n , 1 \le b \le m $

对于 $30\%$ 的分数，$n,m\le 100$。

翻译来自于 [LibreOJ](https://loj.ac/p/2171)。

```input1
2 4 3 15 4
1 1
2 3
1 4
1 3
```

```output1
3 12
1 4 0
2 3 0
1 1 3
```

