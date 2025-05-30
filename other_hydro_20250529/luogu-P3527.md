## 题目描述
Byteotian Interstellar Union (BIU) has recently discovered a new planet in a nearby galaxy.  The planet is unsuitable for colonisation due to strange  meteor showers, which on the other hand make it an exceptionally interesting  object of study.

The member states of BIU have already placed space stations close to the  planet's orbit.  The stations' goal is to take samples of the rocks flying by.

The BIU Commission has partitioned the orbit into $m$ sectors, numbered  from $1$ to $m$, where the sectors $1$ and $m$ are adjacent.  In each sector  there is a single space station, belonging to one of the $n$ member states.

Each state has declared a number of meteor samples it intends to gather before  the mission ends.  Your task is to determine, for each state, when it can  stop taking samples, based on the meter shower predictions for the years to  come.




## 输入格式
The first line of the standard input gives two integers, $n$ and $m$ ($1\le n,m\le 300\ 000$), separated by a single space, that denote,respectively, the number of BIU member states and the number of sectors    the orbit has been partitioned into.

In the second line there are $m$ integers $o_i$ ($1\le o_i\le n$),separated by single spaces, that denote the states owning stations in    successive sectors.

In the third line there are $n$ integers $p_i$ ($1\le p_i\le 10^9$),separated by single spaces, that denote the numbers of meteor samples that the successive states intend to gather.

In the fourth line there is a single integer $k$ ($1\le k\le 300\ 000$) that denotes the number of meteor showers predictions. The following $k$ lines specify the (predicted) meteor showers chronologically. The $i$-th of these lines holds three integers $l_i,r_i,a_i$ (separated by single spaces), which denote that a meteor shower is expected in sectors $l_i,l_{i+1},...,r_i$(if $l_i\le r_i$) or sectors $l_i,l_{i+1},...,m,1,...,r_i$ (if $l_i>r_i$) , which should provide each station in those sectors with $a_i$ meteor samples ($1\le a_i\le 10^9$).


## 输出格式
Your program should print $n$ lines on the standard output.

The $i$-th of them should contain a single integer $w_i$, denoting the number of shower after which the stations belonging to the $i$-th state are    expected to gather at least $p_i$ samples, or the word NIE (Polish for no) if that state is not expected to gather enough samples in the foreseeable future.


## 题目大意
Byteotian Interstellar Union 

有 $n​$ 个成员国。现在它发现了一颗新的星球，这颗星球的轨道被分为 $m​$ 份（第 $m​$ 份和第 $1​$ 份相邻），第 $i​$ 份上有第 $a_i​$ 个国家的太空站。

这个星球经常会下陨石雨。BIU 已经预测了接下来 $k$ 场陨石雨的情况。

BIU 的第 $i$ 个成员国希望能够收集 $p_i$ 单位的陨石样本。你的任务是判断对于每个国家，它需要在第几次陨石雨之后，才能收集足够的陨石。

#### 输入格式

第一行是两个数 $n,m$。

第二行有 $m$ 个数，第 $i$ 个数 $o_i$ 表示第 $i$ 段轨道上有第 $o_i$ 个国家的太空站。

第三行有 $n$ 个数，第 $i$ 个数 $p_i$ 表示第 $i$ 个国家希望收集的陨石数量。

第四行有一个数 $k$，表示 BIU 预测了接下来的 $k$ 场陨石雨。 接下来 $k$ 行，每行有三个数 $l_i,r_i,a_i$ ，表示第 $k$ 场陨石雨的发生地点在从 $l_i$ 顺时针到 $r_i$ 的区间中（如果 $l_i \leq r_i$，则是 $l_i, l_i + 1 
\cdots, r_i$，否则就是 $l_i, l_i + 1, 
\cdots m - 1, m, 1, 2, \cdots r_i$），向区间中的每个太空站提供 $a_i$ 单位的陨石样本。

#### 输出格式

输出 $n$ 行。第 $i$ 行的数 $w_i$ 表示第 $i$ 个国家在第 $w_i$ 波陨石雨之后能够收集到足够的陨石样本。如果到第 $k$ 波结束后仍然收集不到，输出 `NIE`。

#### 数据范围

$1\le n,m,k\le 3\cdot10^5$；

$1\le p_i,a_i\le 10^9$；

```input1
3 5
1 3 2 1 3
10 5 7
3
4 2 4
1 3 1
3 5 2
```

```output1
3
NIE
1
```

