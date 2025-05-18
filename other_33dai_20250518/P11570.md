## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/wv3r15c6.png)


## 题目描述
给定一个长为 $n$ 的序列 $bot$。

有 $q$ 次询问，每次给出三个数 $l,x,y$，请你求出有多少个以 $l$ 为左端点的区间 $[l,r]$（$l\le r$）使得 $\text{mex}(\{bot_l,bot_{l+1},\cdots,bot_r\})\in[x,y]$。

注：一个可重集合 $S$ 的 $\text{mex}$ 函数 $\text{mex}(S)$ 指的是**最小**的没有在 $S$ 中出现过的**非负整数**，如 $\text{mex}(\{0,1,1,3\}) = 2$。 

## 输入格式
第一行两个正整数 $n,q$，表示序列的长度和询问的次数。

第二行 $n$ 个数，表示序列 $bot$。

接下来 $q$ 行，每行三个整数 $l,x,y$。

## 输出格式
输出共 $q$ 行，每行一个整数，表示答案。



```input1
4 2
0 1 3 2
1 2 2
2 1 4
```

```output1
2
0
```

```input2
10 10
0 0 1 1 1 0 0 1 0 1
1 0 0
2 0 1
3 1 2
4 0 1
5 0 2
6 0 1
7 1 1
8 2 2
9 0 0
10 1 2

```

```output2
0
1
5
2
6
2
1
2
0
0

```

## 提示
对于 $100\%$ 的数据，$1\le n,q \le 3\times 10^5$，$0\le bot_i < n$，$0\le x \le y \le n$，$1 \le l\le n$。

**本题采用捆绑测试。**

+ Subtask 1(10pts)：$n,q\le 300$。
+ Subtask 2(15pts)：$n,q\le 2000$。
+ Subtask 3(15pts)：$bot_i \le 1$。
+ Subtask 4(20pts)：$x=y$。
+ Subtask 5(40pts)：无特殊限制。

