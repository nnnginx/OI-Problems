## 题目背景

译自 [Izborne Pripreme 2016 (Croatian IOI/CEOI Team Selection)](https://hsin.hr/pripreme2016/) D1T2。$\texttt{4s,0.5G}$。


为了卡掉理论复杂度较劣的解法，在 Subtask 0 添加了 Hack 数据（#35~#39，感谢 @Hoks 和 @N_z_），同时将时限改为 1.5s。欢迎对数据的加强。


## 题目描述

给定字符串 $s$。

定义 $s(l,r)$ 为 $s$ 第 $l\sim r$ 个字符组成的字符串。

定义 $t(l,r)$ 为 $s$ 删除第 $l\sim r$ 个字符后得到的字符串。

找到最长的区间 $[l,r]$，使得 $s(l,r)$ 在 $t(l,r)$ 中作为子串出现。


## 输入格式
一行一个字符串 $s$。


## 输出格式
输出一个整数，表示最长可能的区间长度。  


```input1
abcxyzabc

```

```output1
3
```

```input2
bbcdbcbbcbadadda
```

```output2
5
```

## 提示

#### 样例解释

不难注意到 $\texttt{bbcdbcb\underline{bcbad}adda} \to \texttt{bbcd\underline{bcbad}da}$。

#### 数据范围

对于 $100\%$ 的数据，保证：

- $1\le |s| \le 10^5$；
- $s$ 中只有小写字母。


| 子任务编号 | $\vert s\vert \in $ | 得分 |  
| :--: | :--: | :--: | 
| $ 1 $    | $ [1,400] $    |   $ 16 $   |  
| $ 2 $    | $ (400,5000] $   |  $ 24 $   |  
| $ 3 $    | $ (5000,10^5]$ | $ 60 $   |  



