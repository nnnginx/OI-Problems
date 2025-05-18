## 题目背景

译自 [Izborne Pripreme 2015 (Croatian IOI/CEOI Team Selection)](https://hsin.hr/prip15/) D1T1。$\texttt{2s,0.5G}$。

## 题目描述

给定 $n$ 个二维笛卡尔坐标系中的向量 $v_i=(x_i,y_i)$。

令点 $P_0=(1,1)$。对于 $1\le i\le n$，有 $P_i=P_{i-1}+v_i$。

有一个变量 $\mathrm{pos}$，初始时为 $1$。有 $m$ 个操作：

- $\texttt{B}$：令 $\mathrm{pos}\gets\max(1,\mathrm{pos}-1)$。
- $\texttt{F}$：令 $\mathrm{pos}\gets\min(n,\mathrm{pos}+1)$。
- $\texttt{C}$ $x$ $y$：令 $v_{\mathrm{pos}}\gets (x,y)$。
- $\texttt{Q}$：询问 $\displaystyle \sum_{1\le i\le n} f(i)$，其中 $f(i)$ 表示线段 $P_{i-1}P_i$ 与坐标轴相交了多少次。
    - **特别地，若 $P_{i-1}P_i$ 经过原点，我们也认为与两个坐标轴都相交。**

这里，**保证任意时刻，对于 $\forall 1\le i\le n$，都有 $x_i,y_i$ 是偶数。**



## 输入格式

第一行，一个正整数 $n$。

接下来 $n$ 行，每行两个**偶数** $x_i,y_i$。

第 $(n+2)$ 行，一个正整数 $m$。

接下来 $m$ 行，每行先是一个大写字母，再是零个或两个**偶数**，描述一个操作。格式见题目描述处。

## 输出格式

对于每个查询操作，输出一行一个非负整数表示答案。

```input1
6
2 2
2 -6
-2 -4
-6 4
10 -10
-8 12
16
Q
C -4 -4
F
F
Q
F
C 6 -2
B
B
B
Q
C 0 6
Q
F
C -8 4
Q
```

```output1
4
4
3
1
5
```

```input2
5
6 2
0 -6
-2 2
-6 -8
4 0
12
Q
C 4 4
Q
F
F
F
C -6 -2
Q
B
B
C -4 -6
Q
```

```output2
3
5
5
4
```

## 提示


对于 $100\%$ 的数据，保证：

- $1\le n\le 10^5$，$1\le n\le 3\times 10^5$；
- $|x|,|y|,|x_i|,|y_i|\le 500$，且**均为偶数**。


| 子任务编号 | $n\le $ |  $m\le $ |  得分 |  
| :--: | :--: | :--: |  :--: |    
| $ 1 $    | $ 1\, 000 $    |  $1\, 000$ |$ 9 $   |  
| $ 2 $    | $ 5\times 10^4 $   |  $ 10^5 $ |  $ 35 $   |  
| $ 3 $    | $ 10^5 $ | $ 3\times 10^5 $ |  $ 56 $   |  


