

## 题目描述

一家缩写为 LLL 的公司正在设计 logo，他们的初步方案是在一张方格上放置三个 L 形的图案以及一些额外的装饰性图形。例如：

![](./3484/file/pic2.png)

（灰色区域表示装饰性图形）

三个 L 图案和装饰性图形均放置在方格之中，且必须占满方格，“L”的横竖笔画长短均可，但长度必须大于零（即不能退化为一条线段）。另外，为了使 L 图形醒目且容易识别，设计师规定三个 L 形图案之间不能有重叠或交叉的部分。当然，L 形图案也不能穿过装饰图形或与之重叠。

现在设计师已经确定了所有装饰性图形的位置，希望你计算一下放置不同的 L 形图案总共可以设计出多少个 logo。

## 输入格式

输入文件第一行包含两个空格分开的正整数 $n$ 和 $m$，分别表示方格的行数和列数。
接下来 $n$ 行，每行 $m$ 个字符，为 $\texttt{"."}$ 或 $\texttt{"\#"}$。$\texttt{"\#"}$ 表示该方格为装饰性图形，$\texttt{"."}$ 表示可以放置 L 图案的空白区域。

## 输出格式

输出一个整数，为可能的 logo 总数。

```input1
4 4
....
#...
....
..#.
```

```output1
4
```

## 数据规模与约定

对于 $100\%$ 的数据，$2\le n,m\le 30$。

## 题目来源

NOI2015 重庆市选

