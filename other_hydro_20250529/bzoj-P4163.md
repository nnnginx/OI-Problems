## 题目描述

给定四种对字符串 $S$ 的操作：

1. `push_back(P)`：在 $S$ 后连接一个字符串 $P$，即 $S=S+P$，代价为 $|P|$；

2. `push_front(P)`：在 $S$ 前连接一个字符串 $P$，即 $S=P+S$，代价为 $|P|$；

3. `symmetry_back()`：将 $S$ 翻转后连接在 $S$ 之后，即 $S=S+\operatorname{rev}(S)$，代价为 $1$；

4. `symmetry_front()`：将 $S$ 翻转后连接在 $S$ 之前，即 $S=\operatorname{rev}(S)+S$，代价为 $1$；

给定一个目标串 $S$，要求你通过上述四种操作，用最少的代价合成出目标串，初始只有一个空串。

## 输入格式

第一行一个正整数 $T$，表示数据组数。

接下来 $T$ 行，每组数据一行，为字符串 $S$。

## 输出格式

每组数据一行输出一个正整数表示最少的代价。

```input1
7 
c
aaaab
bbaaaacc
ababa
abba
baab
aaabacdbbdcabaaaaaaaaaaaab
```

```output1
1 
4 
7 
5 
3 
3
18
```

## 样例解释

`{} -> c`，代价为 $1$；

`{} -> aa -> aaaa -> aaaab`，代价为 $2 + 1 + 1 = 4$；

`{} -> aa -> aaaa -> aaaacc -> bbaaaac`，代价为 $2 + 1 + 2 + 2 = 7$；

`{} -> ababa`，代价为 $5$；

`{} -> ab -> abba`，代价为 $2 + 1 = 3$；

`{} -> ab -> baab`，代价为 $2 + 1 = 3$；

`{} -> aaa -> aaaaaa -> baaaaaa -> baaaaaaaaaaaab -> aaabacdbbdcabaaaaaaaaaaaab`，
代价为 $3 + 1 + 1 + 1 + 12 = 18$。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq T\leq 10$，$1\leq |S|\leq 10^5$。

