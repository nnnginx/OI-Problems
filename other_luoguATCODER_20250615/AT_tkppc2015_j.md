# AT_tkppc2015_j 仕事をしよう！ (Working!)

## 题目描述

joisino姐姐惊醒时发现自己坐在家里的电视机前，似乎之前一直在做梦。  
但她意识到，从开始看电视到现在已经过去了很长时间，墙上的时钟显示离上班时间只剩一个小时。

幸运的是，joisino姐姐上班的市政府离家很近。  
她悠然地到达了办公室，却突然被告知被调到了道路整备课。

这个城市目前正在进行大规模的城市开发，交通拥堵问题令人担忧。  
因此，市政府让joisino姐姐负责监控交通状况。

现在，市里只有1个都市。  
但随着城市开发的进行，预计会有更多的都市出现。  
新建都市时，会选择一个现有都市，并与之通过一条道路相连。  
所以，如果都市的数量是 $n$，就会有 $n-1$ 条道路。  
最初的都市称为都市0，第 $i(1 \le i)$ 个创建的都市称为都市 $i$，第 $i(1 \le i)$ 条修建的道路称为道路 $i$。

每个都市的人口在变化，因此每条道路的通行时间也随之改变。  
为了提高居民的便利性，还需要知道从某个都市出发到达最远的都市需要的时间。

在这种情况下，joisino姐姐将会收到 $Q$ 个关于都市的查询，  
第 $i(1 \le i \le Q)$ 个查询可能是以下三种情况之一：

- 查询1：新建一个都市，与都市 $A_i$ 通过时间为 $C_i$ 的道路相连。
- 查询2：修改道路 $A_i$ 的通行时间为 $C_i$。
- 查询3：查询从都市 $A_i$ 出发到达最远的都市所需的时间。

对于查询3的情况，必须给出答案。

由于工作繁琐，joisino姐姐想编写一个程序来帮助她完成这些任务。

## 输入格式

输入由以下格式通过标准输入给出：

第一行是一个整数 $Q (1 \le Q \le 5 \times 10^5)$，表示查询数量。

接下来的 $Q$ 行中，第 $i$ 行包含三个整数 $T_i (1 \le T_i \le 3), A_i (0 \le A_i \le 当前存在的都市数量 - 1), C_i$，以空格分隔。
- 当 $T_i = 1$ 时，表示新建一个都市，通过时间为 $C_i (1 \le C_i \le 10^9)$ 的道路与都市 $A_i$ 相连。
- 当 $T_i = 2$ 时，表示将道路 $A_i$ 的通行时间修改为 $C_i (1 \le C_i \le 10^9)$。
- 当 $T_i = 3$ 时，表示查询从都市 $A_i$ 出发到最远的都市所需的时间，忽略 $C_i$。如果只有一个都市，答案为0。

## 输出格式

输出中每行对应一个查询3的答案。  
在所有答案后面输出一个换行符。

## 输入输出样例 #1

### 输入 #1

```
6
1 0 10
1 1 7
3 1 0
2 2 5
1 0 17
3 0 0
```

### 输出 #1

```
10
17
```

## 输入输出样例 #2

### 输入 #2

```
7
3 0 0
1 0 10
2 1 15
1 0 7
1 2 5
1 2 8
3 0 0
```

### 输出 #2

```
405
405
940
```

## 输入输出样例 #3

### 输入 #3

```
10
1 0 234
1 1 354
2 1 145
2 1 456
2 1 51
3 0 0
1 0 352
3 0 0
2 1 234
3 3 0
```

### 输出 #3

```

```

## 说明/提示

### 分值划分

该问题有部分评分：

- 数据集1满足 $Q \le 10^4$，正确处理可得5分。
- 数据集2没有额外限制，正确处理可得155分。

### 示例解释1

下面是处理这些查询的过程：
- 查询1：新建都市1，与都市0通过时间为10的道路相连。
- 查询2：新建都市2，与都市1通过时间为7的道路相连。
- 查询3：查询从都市1出发到最远的都市，需要时间10（到达都市0）。
- 查询4：将道路2的通行时间修改为5。
- 查询5：新建都市3，与都市0通过时间为17的道路相连。
- 查询6：查询从都市0出发到最远的都市，需要时间17（到达都市3）。

处理完所有查询后的城市结构如下图所示：  
![](https://img/other/tsukukoma2015/asasffewe/g7.jpg)

### 示例解释2

``` 
0
15
```

在这个例子中，发生了以下事情：
- 查询1：从都市0出发，没有其他都市，输出0。
- 查询2：新建都市1，��都市0通过时间为10的道路相连。
- 查询3：将道路1的通行时间修改为15。
- 查询4：新建都市2，与都市0通过时间为7的道路相连。
- 查询5：新建都市3，与都市2通过时间为5的道路相连。
- 查询6：新建都市4，与都市2通过时间为8的道路相连。
- 查询7：查询从都市0出发到最远的都市，需要时间15（到达都市1或都市4）。

处理完所有查询后的城市结构如下图所示：  
![](https://img/other/tsukukoma2015/asasffewe/g8.jpg)

 **本翻译由 AI 自动生成**