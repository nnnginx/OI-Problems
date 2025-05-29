## 题目描述

给一个 $p\times q\times r$ 的立方体，它由 $p\times q\times r$ 个 $1\times 1\times 1$ 的小立方体构成。每个立方体要么被虫蛀，要么不被。现在郑爽要选出一个 $a\times a\times b$ 的立方体，使得它没有被虫蛀过，并且 $4\times a\times b$ 最大。

## 输入格式

第一行是 $p,q,r$。

以下 $p\times q$ 行，每行 $r$ 个字符，$(x,y,z)$这个格子出现在输入的第 $1 + (y \times p + x - p)$行的第 $z$ 个字符。`N` 代表未被虫蛀，`P` 代表被虫蛀了。

## 输出格式

仅一行，代表郑爽需要的最大的 $4\times a\times b$。

## 样例

```input1
3 2 5
PNNNN
PNNNN
NPPNP
PNNNP
NNNNP
PPNNP
```

```output1
24
```

## 数据规模与约定

对于 $100\%$ 的数据：$p,q,r\leq 150$。

## 题目来源

Baltic2009