## 题目描述
你有一个 $N\times N$ 的棋盘，每个格子内有一个整数，初始时的时候全部为 $0$，现在需要维护两种操作：

命令|参数限制|内容|
:-:|:-:|:-:|
`1 x y A`| $1\le x,y\le N$，$A$ 是正整数|将格子（$x,y$）里的数字加上 $A$
`2 x1 y1 x2 y2`| $1\le x1 \le x2 \le N$，$1\le y1 \le y2 \le N$ |输出 （$x1,y1$）,（$x2,y2$）这个矩形内的数字和。
`3` |无|终止程序

## 输入格式
输入文件第一行一个正整数 $N$。

接下来每行一个操作。

## 输出格式

对于每个 $2$ 操作，输出一个对应的答案。

```input1
4
1 2 3 3
2 1 1 3 3
1 1 1 1
2 1 1 0 7
3
```

```output1
3
0
```

## 数据范围

对于 $100\%$ 的数据满足，$1 \le N \le 5 \times 10^5$，操作次数不超过 $2 \times 10^5$ 个，答案在 `int` 范围内。