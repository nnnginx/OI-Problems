## 题目背景
Ana 的几个朋友要过来参加烙饼。
## 题目描述
Ana 的朋友们将在 $T$ 分钟以内到达，这时 Ana 发现她没有面粉、牛奶、鸡蛋和果酱这四种必备的配料。她于是开车在附近购买这些配料。

Ana 的街区有 $n$ 个路口，编号为 $1\sim n$，还有 $m$ 条**单行道**将这些路口连接起来。Ana 从 $1$ 号路口出发每条路上都有一家卖一些配料（可能全部都有）的商店。

如果 Ana 不在商店前停车，她将需要用 $1$ 分钟在任何道路上行驶，否则她将用 $2$ 分钟购买店内**所有原料**，然后开车到路口。Ana 喜欢比较每个商店的配料的价格，所以**尽管她已经拥有了所有的原料，她也可以进商店**。

例如说，以下是一个街区的例子，有 $5$ 个路口，用 $7$ 条路连接起来。

![](./11697/file/5jFWypRS.png)

Ana 有五个购买配料的方案，具体见下表：

![](./11697/file/YWVy2JXq.png)

请编写一个程序，计算 Ana 在 $T$ 分钟及以内购买配料并回到家（$1$ 号路口）的方案数。由于答案可能很大，你只需要输出**答案模 $5557$ 的结果**。
## 输入格式
输入共 $m+2$ 行。

第一行两个整数 $n,m$，分别表示路口个数和道路条数。  
第 $2\sim m+1$ 行，每行两个正整数 $u,v$ 和一个字符串 $s$，描述一条从 $u$ 到 $v$，并且能够购买配料 $s$ 的单行道。  
第 $m+2$ 行一个整数 $T$，表示 Ana 的朋友们将要到达的时间，单位为分钟。

字符串 $s$ 仅包含以下四种字符：

- `B`，代表面粉；
- `J`，代表鸡蛋；
- `M`，代表牛奶；
- `P`，代表果酱。
## 输出格式
输出仅一行一个整数，表示 Ana 在 $T$ 分钟及以内购买配料并回到家（$1$ 号路口）的方案数模 $5557$ 的结果。

```input1
3 3
1 2 BMJ
2 3 MJP
3 1 JPB
5
```

```output1
3
```

```input2
3 4
1 2 B
2 1 P
1 3 J
3 1 M
8
```

```output2
2
```

```input3
5 7
1 2 B
2 4 M
1 3 J
3 4 MB
4 1 JP
4 5 J
5 1 P
7
```

```output3
5
```
## 提示
**【样例 3 解释】**

样例 3 即为题面中给出的例子，请自行看题面理解。

**【数据范围】**

对于所有数据，满足 $1\leqslant u,v\leqslant  n\leqslant 25$，$1\leqslant m\leqslant 500$，$1\leqslant T\leqslant 10^9$。

**【题目来源】**

本题来源自 **_[COCI 2009-2010](https://hsin.hr/coci/archive/2009_2010/) [CONTEST 4](https://hsin.hr/coci/archive/2009_2010/contest4_tasks.pdf) T6 PALACINKE_**，按照原题数据配置，满分 $130$ 分。

由 [Eason_AC](https://www.luogu.com.cn/user/112917) 翻译整理提供。
