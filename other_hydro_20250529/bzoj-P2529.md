## 题目描述

给出若干木棍，每根木棍有特定的颜色和长度。问能否找到三条颜色不同的木棍构成一个三角形（注意这里所说的三角形面积要严格大于 $0$）。

## 输入格式

第一行给出一个整数 $k$（$3\leq k\leq 50$），表示颜色的种数。这 $k$ 种颜色被标号为 $1$ 至 $k$。

接下来 $k$ 行，第 $i+1$ 行描述颜色为 $i$ 的木棍的信息。

首先一个整数 $N_i$（$1\leq N_i\leq 10^6$）表示颜色为 $i$ 的木棍的数量。

接下来 $N_i$ 个整数，表示这 $N_i$ 根木棍各自的长度。

所有木棍的长度 $\leq 10^9$。总木棍数量 $\leq 10^6$。

## 输出格式

你的程序应该仅输出一行。

如果有解，输出六个整数，分别表示第一条边的颜色，第一条边的长度，第二条边的颜色，第二条边的长度，第三条边的颜色，第三条边的长度，这六个整数以空格分割。

如果有多组解，随便输出一组即可。

如果无解，输出 `NIE`。

```input1
4
1 42
2 6 9
3 8 4 8
1 12
```

```output1
3 8 4 12 2 9
```

## 提示

鸣谢 Kac。