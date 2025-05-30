## 题目描述

在某一天，你有了一个女性朋友。

你打算利用 $k$ 天时间陪她，每天有很多种娱乐方式可供选择，你需要从中选择一种进行（一天只能进行一个项目），比如说一起去看电影、一起去主题公园，一起去逛街等等，一共 $n$ 种项目。当然每个项目重复太多次你都会觉得无聊，因此第 $i$ 个项目最多进行 $c_i$ 次。你虽然智商很高，但是情商堪忧，即使这些你准备的活动都是希望让她开心的，不过由于你笨拙的语言表达和过于理智的行动，可能使这些活动出现意外。经过你悉心的计算，你发现如果某一天进行了第 $i$ 个项目，如果一切顺利的话她应该是很高兴的，但她会有 $a_i$ 的概率不高兴。如果她本来是很高兴的，但突然今天你让她不高兴了，她就会觉得很失落，并且对你的好感度大大下降。你希望尽可能避免这种情况发生，因此你要安排这 $k$ 天之内每天进行的项目，最小化她感到失落的期望次数。

你的女性朋友十分在意你，所以她的心情只会因为你发生改变。第一天之前，因为你没有邀请她进行任何活动，所以她是不高兴的。

## 输入格式

第一行有一个非负整数 $t$，表示一共有 $t$ 组数据。

对于每组数据，第一行有两个非负整数 $n,k$，分别表示你准备的项目个数和你用来陪她的天数。（$n\le 10^5$，$k\le10^9$）

接下来 $n$ 行，每一行描述一个项目，形如“$x_i$ $y_i$ $c_i$”且三个数均为非负整数，表示进行完这个项目之后她有$\frac{x_i}{y_i}$的概率不高兴，并且这个项目只能进行不超过 $c_i$ 次。（$x_i,y_i\le 10^4,c_i\le 10^9$）

## 输出格式

一共 $t$ 行，对于每组数据输出使她感到失落的最小期望次数，四舍五入保留 $6$ 位小数。

```input1
3
1 2
0/1 3
1 2
1/1 3
1 2
1/2 3
```

```output1
0.000000
0.000000
0.250000
```

## 样例说明

考虑第三组数据，因为只有一个项目所以只好每天都安排这个。

在第一天之前她总是不高兴的，一共有：

第一天不高兴，第二天也不高兴、

第一天高兴，第二天不高兴、

第一天不高兴，第二天高兴、

第一天不高兴，第二天也不高兴，

这四种情况，又因为每天的项目让她高兴或者是不高兴的概率都是0.5，因此这四种情况是等概率发生的。

只有在第二种情况下，她会感到失落一次。

因此答案是 $(1*1+0*3)\div 4=0.25$。

## 数据范围

对于前 $10\%$ 的数据，$n,k\le 5$。

对于前 $30\%$ 的数据，$n,k\le 7$。

对于前 $40\%$ 的数据，$n,k\le 10$。

对于前 $60\%$ 的数据，$n\le 1000,k\le 10^5$。

对于 $100\%$ 的数据，$n\le 10^5$，$k\le 10^9$，数据组数不会太多，大概不超过 10 组，数据保证分数有意义并且$\sum c_i\le k$。