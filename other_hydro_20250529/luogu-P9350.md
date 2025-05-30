## 题目描述
There are $N$ residents in JOI Kingdom, numbered from $1$ to $N$. Resident $i$ ($1\le i\le N$) lives at the coordinate $X_i$ on the real line, and its **power of influence** is $E_i$. It may be the case that more than one residents live at the same coordinate. A resident with a large power of influence has a high advertising potential. But such a resident is careful in buying books.

Rie published a book on informatics. In order to encourage many people to buy copies of the book, she can donate copies of the book to some residents. If she donates a copy of the book to Resident $i$ ($1\le i\le N$), Resident $i$ will get a copy of Rie’s book. Moreover, among the residents who did not yet get copies of the book, every resident $j$ ($1\le j\le N$) satisfying the following condition will buy a copy of the book and get it.

-  The distance between Resident $i$ and Resident $j$ on the real line is less than or equal to $E_i - E_j$. In other words, $|X_i − X_j| \le E_i − E_j$ is satisfied.

If all the residents read Rie’s book, the Olympiads in Informatics will be greatly recognized. Write a program which calculates the minimum number of residents who will be donated copies of Rie’s book so that all the residents in JOI Kingdom will get copies of Rie’s book.

## 输入格式
Read the following data from the standard input.

> $N$  
> $X_1$ $E_1$  
> $X_2$ $E_2$  
> $\vdots$  
> $X_N$ $E_N$

## 输出格式
Write one line to the standard output. The output should contain the minimum number of residents who will be donated copies of Rie’s book.

## 题目大意
JOI 王国有 $N$ 位居民，从 $1$ 到 $N$ 编号。居民 $i$（$1\le i\le N$）居住在数轴上坐标 $X_i$ 处，其**影响力**为 $E_i$。同一个坐标可能住了多于一位居民。居民的影响力越高，广告效应也越高，但买书也越谨慎。

Rie 出版了一本关于信息学的书。为了让更多人购买这本书，她可以给一些居民送书。如果她给居民 $i$（$1\le i\le N$）送了一本书，除了居民 $i$ 将得到一本 Rie 的书外，在还没有得到这本书的居民中，每一个满足以下条件的居民 $j$（$1\le j\le N$）都会购买这本书：

- 居民 $i$ 和 居民 $j$ 在数轴上的距离小于或等于 $E_i - E_j$。换句话说，$|X_i - X_j| \le E_i - E_j$ 成立。

如果所有的居民都读了 Rie 的书，信息学竞赛将得到极大的认可。请写一个程序，计算 Rie 最少将书赠送给多少位居民，就可以让 JOI 王国的所有居民都会得到 Rie 的书。

```input1
4
4 2
2 3
3 4
6 5

```

```output1
2

```

```input2
3
7 10
10 10
7 10

```

```output2
2

```

```input3
10
31447678 204745778
430226982 292647686
327782937 367372305
843320852 822224390
687565054 738216211
970840050 766211141
563662348 742939240
103739645 854320982
294864525 601612333
375952316 469655019

```

```output3
5
```

## 提示
## Samples

### Sample 1

For example, if Rie donates copies of the book in the following way, all the residents in JOI Kingdom will get copies of Rie’s book.

- Rie donates a copy of the book to Resident 3.
  - Since $|X_3 - X_1| = 1$ and $E_3 - E_1 = 2$, Resident 1 will buy a copy of Rie’s book and get it.
  - Since $|X_3 - X_2| = 1$ and $E_3 - E_2 = 1$, Resident 2 will buy a copy of Rie’s book and get it.
  - Since $|X_3 - X_4| = 3$ and $E_3 - E_4 = -1$, Resident 4 will not buy a copy of Rie’s book.
  Therefore, Residents 1, 2, 3 will get copies of Rie’s book.
- Rie donates a copy of the book to Resident 4. Since all the residents except Resident 4 already got copies of Rie’s book, all the residents in JOI Kingdom finally get copies of Rie’s book.

Since it is impossible to donate copies of the book to less than two residents so that all the residents in JOI Kingdom will get copies of Rie’s book, output 2.

This sample input satisfies the constraints of Subtasks 2, 3, 4.

### Sample 2

This sample input satisfies the constraints of all the subtasks.

### Sample 3

This sample input satisfies the constraints of Subtasks 2, 3, 4.

## Constraints

- $1\le N\le 5\times 10^5$.
- $1\le X_i\le 10^9$ ($1\le i\le N$).
- $1\le E_i\le 10^9$ ($1\le i\le N$).
- Given values are all integers.

## Subtasks

1. (10 points) $E_1=E_2=\cdots=E_N$.
2. (23 points) $N\le 16$.
3. (36 points) $N\le 10^3$.
4. (31 points) No additional constraints.


