# AT_iroha2019_day4_b 叫び声

## 题目背景

一个刺破黑暗的尖叫声，使我和伊吕波都立刻察觉到外面的异常。远处正剧烈摇动的城市闪烁着红光，发出着轰鸣的异响。“那是什么……”，当我意识到危险的时候，伊吕波已经开始奔跑了。

## 题目描述

在伊吕波所在的城市中，有 $M+1$ 个车站，编号从 $1$ 到 $M+1$，还有 $N$ 辆电车。

现在的时间为 $0$，伊吕波现在位于第 $1$ 个车站，并打算前往第 $M+1$ 个车站。

第 $i$ 辆电车在时间 $A_i$ 时从第 $1$ 个车站出发，电车到达第 $j+1$ 个车站的时间是 $A_i + B_i \times j$。（$1 \leq j \leq M$）

此外，伊吕波可以通过步行从第 $k$ 个车站到第 $k+1$ 个车站，每段车站之间的步行时间是 $L$。（$1 \leq k \leq M$）

伊吕波可以在车站更换交通工具，换车时不会耗费时间。她只能在车站之间换车，不能在其他地方换车。

请求出伊吕波从第 $1$ 个车站到第 $M+1$ 个车站的最短到达时间。

## 输入格式

第一行有三个整数 $N,M,L$，含义如题所述。 

接下来的 $N$ 行，每行包含两个整数 $A_i$ 和 $B_i$，含义如题所述。

## 输出格式

一行一个整数，表示伊吕波从第 $1$ 个车站到第 $M+1$ 个车站的最短到达时间。

## 输入输出样例 #1

### 输入 #1

```
3 3 4
4 2
2 3
3 4
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
3 3 3
4 2
2 3
3 4
```

### 输出 #2

```
9
```

## 输入输出样例 #3

### 输入 #3

```
1 100 10
100 1
```

### 输出 #3

```
200
```

## 输入输出样例 #4

### 输入 #4

```
3 139128390 220019821
3162336416461334 196423673
2909210940940890 272140126
31923189201903829 68312342
```

### 输出 #4

```
30490445798837804
```

## 说明/提示

对于 $100\%$ 的数据，保证输入均为整数，$1 \leq N \leq 10^5$，$1 \leq M, L \leq 3 \times 10^8$，$0 \leq A_i \leq 10^{17}$，$1 \leq B_i \leq 3 \times 10^8$。

#### 样例解释 1

通过以下方式，可以在时间 $10$ 时到达第 $4$ 个车站。  
1. 等待第 $2$ 辆电车出发（时间 $0$ 至时间 $2$）
2. 乘坐第 $2$ 辆电车到达第 $2$ 个车站（时间 $2$ 至时间 $5$）
3. 等待第 $1$ 辆电车出发（时间 $5$ 至时间 $6$）
4. 乘坐第 $1$ 辆电车到达第 $4$ 个车站（时间 $6$ 至时间 $10$）

#### 样例解释 2

直接跑到第 $4$ 个车站（时间 $0$ 至时间 $9$），可以在时间 $9$ 时到达第 $4$ 个车站。 

#### 样例解释 3

通过以下方式移动，可以在时间 $200$ 时到达第 $101$ 个车站。  
1. 跑到第 $2$ 个车站（时间 $0$ 至时间 $10$）
2. 跑到第 $1$ 个车站 （时间 $10$ 至时间 $20$）
3. 跑到第 $4$ 个车站 （时间 $20$ 至时间 $50$）
4. 在第 $4$ 个车站  停留 20 个单位时间（时间 $50$ 至时间 $70$）
5. 跑到第 $1$ 个车站 （时间 $70$ 至时间 $100$）
6. 乘坐第 $1$ 辆电车到达第 $101$ 个车站 （时间 $100$ 至时间 $200$）