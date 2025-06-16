## 题目描述

Tao Yuanming(365-427) was a Chinese poet of Eastern Jin dynasty. One of his most famous works is "Peach Blossom Spring", which is a fable about a chance discovery of an ethereal village where the people lead an ideal existence in harmony with nature, unaware of the outside world for centuries. So in Chinese, "Peach Blossom Spring" means "utopia".

In the story of "Peach Blossom Spring", there was a mysterious place. In Qin dynasty, some people escaped to that place during the civil unrest and built a village. They and their descendants never left and never had any contact with the outside world since then, until centuries latter a fisherman of Jin dynasty found them.

Recently, some Chinese ACMers happened to find the relics of the village mentioned in"Peach Blossom Spring".

They also found a document about building hiding places to escape from Qin army. The document said:

There were $n$ houses and $m$ roads in the village. Each road connected two houses. These houses were numbered from $1$ to $n$. There were $k$ families, each living in a different house. 

The houses they lived were house $1$, house $2$, … , house $k$. There were also $k$ broken houses: house $n-k+1$, house $n-k+2$, ... , house $n$, with secret basements so that those houses could be used as hiding places.

The problem was that all roads were broken. People wanted to repair some roads so that every family could reach a hiding place through the repaired roads. Every hiding place could only hold one family. Each road cost some labor to be repaired. The head of the village wanted to find out the minimum cost way of repairing the roads, but he didn't know how to do.

Would you solve the problem which the ancient village head never solved?

## 输入格式

the first line begins with three integers ---- the above mentioned $n, m$ and $k$. Then $m$ lines follow, each containing three integers $u,v$ and $w$, indicating that there is a broken road connecting house $u$ and $v$, and the cost to repair that road is $w$.

## 输出格式

if you cannot find a proper way to repair the roads, output $-1$ in a line. Otherwise, output the minimum cost to repair
the roads in a line.

```input1
4 3 1
4 2 10
3 1 9
2 3 10
```

```output1
29
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 7\times 10^3$，$0\le m\le 10^4$，$1\le k\le 5$，$2k\le n$，$1\le w\le 10^3$。