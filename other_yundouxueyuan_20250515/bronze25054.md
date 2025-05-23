# 外卖

奶龙又点了 $n$ 份外卖，但是他不喜欢重量相同的外卖，所以他会不断找到两个重量相同的外卖把他们合并在一起。 形式化地，有一个序列 $a$，奶龙会找到满足 $a_i=a_j$的最小的$a_i$, 以及其对应的最小的两个下标$i$, $j$ $(i < j)$，删除$a_i$，并令$a_j= a_j+a_i$。请你求出来，奶龙不断进行这样的操作后，最终得到的每个外卖的重量。

### 输入格式

第一行一个正整数,表示外卖数量 $n$；

第二行$n$ 个整数，第 $i$ 个整数代表第 $i$ 个外卖的重量 $a_i$。
    

### 输出格式

第一行，输出最终的外卖数量；

第二行，按顺序输出每个外卖的重量。

## 样例

### 样例输入 #1

```
7
3 4 1 2 2 1 1
```

### 样例输出 #1

```
4
3 8 2 1 
```

### 样例输入 #2

```
5
1 1 3 1 1
```

### 样例输出 #2

```
2
3 4 
```

### 样例输入 #3

```
5
10 40 20 50 30
```

### 样例输出 #3

```
5
10 40 20 50 30 
```

### 数据范围与约定

对于 $20\%$ 的数据，保证 $\forall i\neq j, a_i \neq a_j$；

对于 $40\%$ 的数据，$n\leq 5000$；

对于 $100\%$ 的数据，$1\leq n \leq 2\times 10^5, 1\leq a_i\leq 10^9$。