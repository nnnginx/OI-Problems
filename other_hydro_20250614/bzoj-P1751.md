## 题目描述

Due to recent rains, water has pooled in various places in Farmer John's field, which is represented by a rectangle of $N \times M$ squares. Each square contains either water (`W`) or dry land (`.`).

Farmer John would like to figure out how many ponds have formed in his field. A pond is a connected set of squares with water in them, where a square is considered adjacent to all eight of its neighbors. Given a diagram of Farmer John's field, determine how many ponds he has.

## 输入格式

* Line $1$: Two space-separated integers: $N$ and $M$.
* Lines $2 \sim N + 1$: $M$ characters per line representing one row of Farmer John's field. Each character is either `W` or `.`. The characters do not have spaces between them.

## 输出格式

* Line $1$: The number of ponds in Farmer John's field.

```input1
10 12
W........WW.
.WWW.....WWW
....WW...WW.
.........WW.
.........W..
..W......W..
.W.W.....WW.
W.W.W.....W.
.W.W......W.
..W.......W.
```

```output1
3
```

## 样例说明
There are three ponds: one in the upper left, one in the lower left, and one along the right side.

## 数据规模与约定

对于 $100\%$ 的数据：$1 \leq N \leq 100$，$1 \leq M \leq 100$。

## 题目来源

Usaco2005 qua