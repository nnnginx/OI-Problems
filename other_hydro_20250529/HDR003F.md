## 题目背景

頰滴る　紅い涙

不安定な視界の中

差し出した手を取れたら

あぁ…そんな世界を夢みた

-------

哭いて…

激しく  燃やした 黒い感情 

届かぬ この手に

Cry 闇の中で

最果てから 光へ手を翳して

揺らいだ想いさえも 闇の奥底へ堕ちてく

## 题目描述

出题人在打天地交互的时候爆了一整串的 far ，异常气愤，于是打算出个题散(bao)播(fu)希(she)望(hui)。

设正整数 $n, m$ 互质，$k$ 为整数，定义函数 $F(n, m, k)$ 为小于 $\displaystyle m+n$ 的正整数集合 $\{1, 2, \cdots, m + n - 1\}$ 中，所有满足 $\displaystyle\sum_{x \in S} x \equiv k \pmod n$ 的 $m$ 元子集 $S$ 的个数。

现给定正整数 $N, M, K$，求所有 $F(i,j,x)$ 之积，使得 $1\le i\le N$，$1\le j\le M$，$1\le x\le K$，并且 $i$ 与 $j$ 互质。

由于结果很大，所以你只需要求出结果对特定素数 $p$ 取模的值。

**同时请注意实现程序时常数因子带来的影响。**

## 输入格式

**本题多测。** 每个测试点共有 $T$ 组数据。

第一行两个正整数 $T,p$ 。

接下来 $T$ 行，每行三个正整数 $N, M, K$，由空格分开。

## 输出格式

对于每组数据：一行，一个整数，表示所求的值（对 $p$ 取模）。

```input1
3 1926195307
2 3 3
3 3 3
5 6 1
```
```output1
8
64
363031200
```

## 提示说明

本题采用捆绑测试，分 $5$ 个 Subtask 。

+ 对于 Subtask 1 ~~(Tutorial)~~：
  + $T=1$
  + $1\leq N,M,K\leq 6$
  + $p=10^9+7$。
+ 对于 Subtask 2 ~~(PST 4.0)~~：
  + $T=1$
  + $1\leq N,M,K\leq200$
  + $p=10^9+7$。
+ 对于 Subtask 3 ~~(PRS 7.5)~~：
  + $T=100$
  + $1\leq N,M,K\leq 1000$
  + $p=10^9+7$。
+ 对于 Subtask 4 ~~(FTR 9.8)~~：
  + $T=10^3$
  + $1 \leq N,M,K\le 10^5$
  + $10^9\le p\le2\times10^9$。
+ 对于 Subtask 5 ~~(BYD ??)~~：
  + $T=9999$
  + $1 \leq N,M,K\le 5\times10^5$
  + $10^9\le p\le2\times10^9$。

Subtask $1\sim5$ 的分值分别为 $5,7,11,17,60$ 。

特别的，假设您在一个测试点中前 $x$ 个询问正确，则您得该测试点的分值的 $\left\lfloor100\times\sqrt\dfrac{x}{T}\right\rfloor\%$ 分。您在任何一个 Subtask 的得分则为对应 Subtask 中所有测试点得分的最小值。

特别的，**TLE 一律不得分。**

**再次提醒注意实现程序时常数因子带来的影响。**

---

She glimpsed the truth of this cage dubbed "reality".

Knowing everything, what exactly would change?
