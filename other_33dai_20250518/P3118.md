## 题目描述
Bessie is out at the movies.  Being mischievous as always, she has decided to hide from Farmer John for L (1 <= L <= 100,000,000) minutes, during which time she wants to watch movies continuously. She has N (1 <= N <= 20) movies to choose from, each of which has a certain duration and a set of showtimes during the day.  Bessie may enter and exit a movie at any time during one if its showtimes, but she does not want to ever visit the same movie twice, and she cannot switch to another showtime of the same movie that overlaps the current showtime.

Help Bessie by determining if it is possible for her to achieve her goal of watching movies continuously from time 0 through time L.  If it is, determine the minimum number of movies she needs to see to achieve this goal (Bessie gets confused with plot lines if she watches too many movies).

## 输入格式
The first line of input contains N and L.

The next N lines each describe a movie.  They begin with its integer duration, D (1 <= D <= L) and the number of showtimes, C (1 <= C <= 1000).  The remaining C integers on the same line are each in the range 0..L, and give the starting time of one of the showings of the movie.  Showtimes are distinct, in the range 0..L, and given in increasing order.


## 输出格式
A single integer indicating the minimum number of movies that Bessie needs to see to achieve her goal. If this is impossible output -1 instead.


## 题目大意
### 题目描述

Bessie 正在外看电影。调皮的她想在 $L$（$1 \leq L \leq 100,000,000$）分钟内连续观看电影来躲避农夫 John。她有 $N$（$1 \leq N \leq 20$）部电影可选，每部电影有特定时长和多个放映场次。Bessie 可以在电影放映期间的任意时刻入场或离场，但不能重复观看同一部电影，也不能切换到同一部电影时间重叠的场次。

请判断 Bessie 是否能从时间 $0$ 到时间 $L$ 连续观看电影。若可行，求出达成目标所需观看的最小电影数量（过多电影会让 Bessie 混淆剧情）。

### 输入格式

第一行输入包含 $N$ 和 $L$。

接下来 $N$ 行描述每部电影：每行以整数时长 $D$（$1 \leq D \leq L$）和场次数 $C$（$1 \leq C \leq 1000$）开头，随后给出 $C$ 个按升序排列的场次开始时间（范围 $0$ 至 $L$，且互不重复）。

### 输出格式

输出达成目标所需的最小电影数量。若不可能则输出 $-1$。

### 说明/提示

Bessie 可以观看第四部电影的首场（时间 $0$ 至 $20$），接着观看第一部电影的首场（时间 $20$ 至 $65$），最后观看第二部电影的末场（时间 $65$ 至 $100$）。

```input1
4 100 
50 3 15 30 55 
40 2 0 65 
30 2 20 90 
20 1 0 

```

```output1
3 

```

## 提示
Bessie should attend the first showing of the fourth movie from time 0 to time 20.  Then she watches the first showing of the first movie from time 20 to time 65.  Finally she watches the last showing of the second movie from time 65 to time 100.


