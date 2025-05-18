## 题目描述
King Byteasar is the ruler of the whole solar system that contains ![](http://main.edu.pl/images/OI17/tel-en-tex.1.png) planets.

This number is so large that people have abandoned the silly custom of naming the planets    and use numbers instead. The planets are thus conveniently numbered from 1 to ![](http://main.edu.pl/images/OI17/tel-en-tex.2.png).

Byteasar's palace is on the planet no. 1, while his military base on the planet no. 2.

A long time ago Byteasar had a teleportation portal established between these two planets,    which allows travelling from either planet to another in two hundred and fifty minutes    (slightly over four hours).

Nowadays the teleportation technology is more mature, and the recent teleportation devices shorten    the travel time to just a single hour. Let us note here, that all the portals, both the Byteasar's old one    and the new ones available on the market, are of course bidirectional, and that the teleportation    travel time is irrespective of the distance travelled.

Some planets of the system are already connected with these new teleportation portals.

In fact, it is already possible to travel between the planets no. 1 and 2 without using the king's private portal,    though this involves several other portals and is thus no faster than the king's portal.

Byteasar finds this rather fortunate, as he believes that such possibility would be a security breach.

The technology itself is increasingly available, and as everyone realises its economic significance,    each pair of planets that are not currently directly connected with a portal are petitioning for establishing    such a connection. Being a wise ruler, Byteasar intends to give his consent to as many constructions as possible,    though keeping himself secure, i.e., not allowing the travel between planets 1 and 2 faster than with his private portal.

Help the king determine how many portals he can agree to.

## 输入格式
Two integers are given in the first line of the standard input, ![](http://main.edu.pl/images/OI17/tel-en-tex.3.png) and ![](http://main.edu.pl/images/OI17/tel-en-tex.4.png)      (![](http://main.edu.pl/images/OI17/tel-en-tex.5.png), ![](http://main.edu.pl/images/OI17/tel-en-tex.6.png)), separated by a single space,      denoting the number of planets in Byteasar's realm and the number of new portals      that already exist.

These teleportation portals are described in the ![](http://main.edu.pl/images/OI17/tel-en-tex.7.png) lines that follow.

Each such line contains two integers ![](http://main.edu.pl/images/OI17/tel-en-tex.8.png) and ![](http://main.edu.pl/images/OI17/tel-en-tex.9.png) (![](http://main.edu.pl/images/OI17/tel-en-tex.10.png)),      separated by a single space, denoting that there is a teleportation portal of the new kind      connecting ![](http://main.edu.pl/images/OI17/tel-en-tex.11.png) and ![](http://main.edu.pl/images/OI17/tel-en-tex.12.png).

No pair of numbers appears twice.

You may assume that the existing network of new portals allows travel from      planet no. 1 to planet no. 2, but in no less than 250 minutes.


## 输出格式
Your program should print out just a single integer, namely the maximum number of portals      Byteasar can agree to without breaching his security.


## 题目大意
### 题目描述

**译自 POI 2010 Stage 2. Day 2「[Teleportation](https://szkopul.edu.pl/problemset/problem/fKO3YZL0f_UM1nHQNDvw7mku/site/?key=statement)」**

现在有 $n$ 个点，目前在 $1$ 号点和 $2$ 号点之间有一条无向边，长度为 $250\min$ 。  
除此之外，还有 $m$ 条无向边，长度都为 $1\ \textrm{h}$ （即 $60\min$）， Byteasar 想知道，还能最多在添加多少条长度为 $1\ \textrm{h}$ 的无向边，使得新图无重边无自环，且 $1$ 号点到 $2$ 号点的最短路仍为 $250\min$ 。

### 输入格式

第一行两个空格隔开的正整数 $n,m$ 。  
接下来 $m$ 行，每行两个空格隔开的正整数 $u_i,v_i$ ，描述原有的边。

### 输出格式

一行一个整数，表示最多添加多少条边，可以使 $1$ 号点到 $2$ 号点的最短路长度保持不变。

翻译来自于 [LibreOJ](https://loj.ac/p/2449)。

```input1
10 10
1 3
3 5
5 7
7 9
2 9
1 4
4 6
6 8
8 10
2 10
```

```output1
10
```

## 提示
数据保证，$2\le n\le 40\ 000$，$0\le m\le 10^6$，$1\le u_i,v_i\le n$，保证只考虑已有的边时， $1$ 号点与 $2$ 号点联通，且最短路长度大于 $250\min$ 。

