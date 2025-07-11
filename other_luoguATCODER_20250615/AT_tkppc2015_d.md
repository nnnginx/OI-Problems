# AT_tkppc2015_d サポーター (Supporter)

## 题目描述

joisino 姐姐在休息结束后，结识了一位冒险者，他们决定一同进入地下城探险。  
途中顺利进行，但意外发生，他们需要迅速赶往一个安全地带。

地下城的每一层都由 $R$ 行 $C$ 列的房间组成，总共 $R \times C$ 个房间，排列成一个网格。  
joisino 姐姐和她的同伴目前位于当前层最西北的房间。  
安全地带位于从当前层向下 $N-1$ 层的最东南的房间。

除了安全地带所在的层以外，每一层都有一些洞。  
洞位于某个房间内，掉入洞中就会降至下一层。在掉落后的位置与掉入位置在同一相对坐标，即以西北角房间为原点向东 $x$ 格、向南 $y$ 格。  
掉落后的房间内不会再有洞，也就是说，进入有洞的房间时，必须掉下去。

每个房间都有一个危险度。  
危险度越高，通过该房间的风险越大。有洞的房间危险度为 $0$，但是掉落后的房间危险度需要计算。  
此时 joisino 姐姐所在房间和安全地带的房间的危险度为 $0$。

joisino 姐姐希望尽可能避免危险，以安全到达安全地带。  
为此，她需要找到一条最短路径（即不向西或北移动），并使路径上的房间危险度总和最小。  
作为一名优秀的程序员，joisino 姐姐决定编写一个程序计算这条路径的危险度总和。

## 输入格式

输入由标准输入给出，格式如下：

> $ N $ $ R $ $ C $\  
> $ S_1 $ $ S_2 $ : $ S_{N*R} $

- 第 $1$ 行包含三个整数 $N$、$R$ 和 $C$，表示层数（$2 \leq N \leq 100$）、每层的行数（$2 \leq R \leq 100$）和列数（$2 \leq C \leq 100$）。
- 下面的 $N \times R$ 行中，第 $K \times R + 1$ 行到第 $(K+1) \times R$ 行描述了第 $K$ 层的信息（$0 \leq K \leq N-1$）。每一层用 $R$ 行表示，每行是一个长度为 $C$ 的字符串，由 `H` 和 `0` 到 `9` 的数字构成。第 $j$ 个字符为 `H` 时，表示该房间有一个洞；为 `0` 表示该房间是起点或终点；数字 $1$ 到 $9$ 表示房间的危险度。

保证对所有输入，至少存在一条通往安全地带的路径。

## 输出格式

输出一行，表示路径上房间危险度总和的最小值，并在末尾换行。

## 输入输出样例 #1

### 输入 #1

```
3 3 3
06H
H14
257
337
15H
2H8
829
653
470
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
2 5 3
013
871
7HH
163
92H
959
248
792
447
550
```

### 输出 #2

```
14
```

## 说明/提示

### 示例解释 1

可以按顺序 南→掉入洞→东→东→掉入洞→南 移动，以使危险度总和最小。

 **本翻译由 AI 自动生成**