## 题目描述
A railroad siding consists of two (dead-end) sidetracks 1 and 2.

The siding is entered by track A, and left by track B (see figure below).

There are ![](http://main.edu.pl/images/OI17/kol-en-tex.1.png) cars on track A, numbered from ![](http://main.edu.pl/images/OI17/kol-en-tex.2.png) to ![](http://main.edu.pl/images/OI17/kol-en-tex.3.png).

They are arranged in such a way that they enter the siding in the order    ![](http://main.edu.pl/images/OI17/kol-en-tex.4.png).

The cars are to be transferred to the siding, so that they leave it by track B    in the order ![](http://main.edu.pl/images/OI17/kol-en-tex.5.png).

Each car is to be transferred once from track A to one of the sidetracks 1 or 2,    and later (possibly after some transfers of the remaining cars) once from that    sidetrack to the track B.

The sidetracks are long enough to store even the longest trains, so there is    no need to worry about their capacity.

## 输入格式
The first line of the standard input holds one integer ![](http://main.edu.pl/images/OI17/kol-en-tex.6.png) (![](http://main.edu.pl/images/OI17/kol-en-tex.7.png))      that denotes the number of cars for transfer.

The second line stores the numbers ![](http://main.edu.pl/images/OI17/kol-en-tex.8.png) that are a permutation of ![](http://main.edu.pl/images/OI17/kol-en-tex.9.png)      (i.e., each ![](http://main.edu.pl/images/OI17/kol-en-tex.10.png) belongs to ![](http://main.edu.pl/images/OI17/kol-en-tex.11.png), and all these numbers are unique),      separated by single spaces.


## 输出格式
The first line of the standard output should contain the word TAK      (yes in Polish) if there is a way of transferring the cars so that they      enter track B in the order ![](http://main.edu.pl/images/OI17/kol-en-tex.12.png), or the word NIE      (no in Polish) if it is impossible.

If the answer is TAK, the second line should give, separated by      single spaces, the numbers of sidetracks (1 or 2) to which successive cars      ![](http://main.edu.pl/images/OI17/kol-en-tex.13.png) are moved in a correct transfer.

If there are several ways of making the transfer, choose one arbitrarily.


## 题目大意
### 题目描述

**译自 POI 2010 Stage 1.「[Kolej](https://szkopul.edu.pl/problemset/problem/TJVrS_hRC8W5Q6ZBW6mETAIm/site/?key=statement)」**

一个铁路包含两个侧线 $1$ 和 $2$ ，左边由 $A$ 进入，右边由 $B$ 出去（如下图所示）。  

![](https://cdn.luogu.com.cn/upload/image_hosting/bdq72qy0.png)

有 $n$ 个车厢在通道 $A$ 上，编号为 $1$ 到 $n$ ，它们按照 $a_1,a_2,\cdots ,a_n$ 的顺序进入侧线，想要按照 $1,2,\cdots ,n$ 的顺序从通道 $B$ 出去。    
他们可以从 $A$ 到 $1$ 或 $2$ ，然后经过一系列转移从 $B$ 出去（不用考虑容量问题）。求是否能够做到，如果可以，请找出一种方案。

### 输入格式

第一行一个正整数 $n$ 。  
第二行 $n$ 个空格隔开的正整数 $a_1,a_2,\cdots a_n$ 。

### 输出格式

第一行一个字符串，如果能够做到，输出 ```TAK``` ，否则输出 ```NIE``` 。  
若能做到，第二行 $n$ 个空格隔开的正整数，表示每个车厢进入的侧线编号。  
如果有多解，输出任意一种。

翻译来自于 [LibreOJ](https://loj.ac/p/2448)。

```input1
4
1 3 4 2
```

```output1
TAK
1 1 2 1
```

## 提示
对于 $100\%$ 的数据，有 $n \le 1 \times 10^5$。

