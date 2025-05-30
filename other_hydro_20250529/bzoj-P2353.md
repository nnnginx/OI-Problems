## 题目描述

平面上给出 $N$ 个矩形，定义平面内的一个矩形是 cool 的，当且仅当这个矩形的四边完全在给出 $N$ 个矩形的边界上（边界相互重合）。现在你想取 $N$ 个 cool 矩形来一一代表这 $N$ 个矩形。

假如你要用一个 cool 矩形来代表矩形 $I$，那么必须满足这个 cool 矩形完全在 $I$ 之内；要求一个 cool 矩形只能代表一个矩形，并且你选出的代表这 $N$ 个矩形的 $N$ 个 cool 矩形之间，两两不覆盖（边界可以重叠）。

问你选出的 $N$ 个 cool 矩形的最小面积和，或者返回 `-1`，表示无解。

## 输入格式

输入文件第一行括一个数字 $N$，

接下来 $4$ 行 $N$ 列，每列依次为 $4$ 个数字 $(x_1,y_1)$， $(x_2,y_2)$ 表示一个矩形的对顶角坐标。

## 输出格式

输出最小面积，或者 `-1`。

## 样例输入 #1
```plain
2
1 0
1 2
3 4
4 3
```

## 样例输出 #1

```plain
3
```

## 样例输入 #2

```plain
2
0 1
0 1
2 3
2 3
```

## 样例输出 #2

```plain
-1
```

## 数据规模与约定

对于 $100\%$ 的数据，$N\le 30$， $|X|,|Y|\le 10^4$。

## 题目来源

2010福建集训