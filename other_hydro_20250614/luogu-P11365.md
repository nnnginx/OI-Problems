## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/pcokv5zr.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/hasy3fee.png)

## 题目描述
给定排列 $a_1,\dots,a_n$，共 $m$ 次询问，第 $i$ 次询问给定 $m_i$ 个区间 $[l_j,r_j],\;1\le j\le m_i$，满足 $1\le l_j\le r_j\le n,\;r_j<l_{j+1}$，你需要求出有几个二元组 $(p,q)$ 满足 $p<q,\;a_p<a_q$，且存在 $1\le u<v\le m_i$ 使得 $l_u\le p\le r_u,\;l_v\le q\le r_v$。

## 输入格式
第一行两个数表示 $n,m$。

接下来一行 $n$ 个数表示 $a_1,\dots,a_n$。

接下来，每个询问第一行为 $m_i$，接下来 $m_i$ 行为 $l_j,r_j$。

## 输出格式
共 $m$ 行，依次为每个询问的答案。

```input1
5 2
5 4 2 3 1
3
1 1
2 3
4 4
2
1 2
3 4
```

```output1
1
0
```

## 提示
Idea：nzhtl1477，Solution：ccz181078，Code：ccz181078，Data：ccz181078

对于 $100\%$ 的数据，满足 $1\le n\le 5\times 10^5$，$1\le \sum\limits_{i=1}^m m_i\le 5\times 10^5$，$m_i\ge 1$，$1\le a_i\le n$，所有数值为整数。

对于 $0\%$ 的数据，满足 $n\le 10^3,\;\sum\limits_{i=1}^m m_i\le 10^3$。

对于另外 $10\%$ 的数据，满足 $m_i\le 10$。

对于另外 $10\%$ 的数据，满足 $m\le 5$。

对于另外 $80\%$ 的数据，无特殊限制。

