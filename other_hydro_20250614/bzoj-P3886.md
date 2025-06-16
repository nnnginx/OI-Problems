## 题目描述

Bessie is out at the movies. Being mischievous as always, she has decided to hide from Farmer John for $L$ minutes, during which time she wants to watch movies continuously. She has $n$ movies to choose from, each of which has a certain duration and a set of showtimes during the day.Bessie may enter and exit a movie at any time during one if its showtimes, but she does not want to ever visit the same movie twice, and she cannot switch to another showtime of the same movie that overlaps the current showtime. Help Bessie by determining if it is possible for her to achieve her goal of watching movies continuously from time $0$ through time $L$. If it is, determine the minimum number of movies she needs to see to achieve this goal (Bessie gets confused with plot lines if she watches too many movies).

**翻译：**

Bessie 要在电影院里呆 $L$ 分钟，这段时间她要看小型电影度过。电影一共 $n$ 部，每部都播放于若干段可能重叠的区间，Bessie 决不会看同一部电影两次。现在问她要看最少几部电影才能度过这段时间？ 

**注：必须看电影才能在电影院里呆着，同时一场电影可以在其播放区间内任意时间入场出场。**

## 输入格式

The first line of input contains $n$ and $L$. The next $n$ lines each describe a movie. They begin with its integer duration, $d$ and the number of showtimes, $c$. The remaining $c$ integers on the same line are each in the range $0...L$, and give the starting time of one of the showings of the movie. Showtimes are distinct, in the range $0...L$, and given in increasing order.

## 输出格式

A single integer indicating the minimum number of movies that Bessie needs to see to achieve her goal. If this is impossible output $-1$ instead.

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

## 样例说明

Bessie should attend the first showing of the fourth movie from time $0$ to time $20$. Then she watches the first showing of the first movie from time $20$ to time $65$. Finally she watches the last showing of the second movie from time $65$ to time $100$.

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le L \le 10^8,1\le n \le 20$，$1\le d \le L,1\le c \le 10^3$。

## 题目来源

Gold & 鸣谢18357