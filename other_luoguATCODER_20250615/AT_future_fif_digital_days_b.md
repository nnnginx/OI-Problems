# AT_future_fif_digital_days_b Polyomino Connection B

## 题目描述

[题目链接]: https://atcoder.jp/contests/future-fif-digital-days/tasks/future_fif_digital_days_b

## 输入格式

无

## 输出格式

无

## 输入输出样例 #1

### 输入 #1

```
50 10 20
0 25
1 0
49 21
49 49
0 43
41 9
26 6
12 32
38 33
13 4
1 1 50
#
2 3 100
###
#..
2 4 112
#...
####
5 2 122
.#
.#
##
#.
#.
3 5 132
..###
###..
.#...
2 7 141
###....
..#####
7 3 150
..#
..#
..#
..#
..#
..#
###
5 6 158
...#..
..####
..#...
###...
.#....
7 5 166
...#.
...#.
...#.
####.
...##
...#.
...#.
5 8 173
...#....
...#....
########
.....#..
.....#..
9 5 180
..#..
..#..
..#..
..#..
#####
..#..
..#..
..#..
..#..
8 7 187
..#....
..#....
..#....
..#....
#######
.#.....
.#.....
.#.....
8 8 194
.......#
.....###
######..
...#....
...#....
...#....
...#....
...#....
5 12 200
.......#....
.......#####
########....
.....#......
.....#......
12 6 206
...#..
...#..
...#..
...#..
...#..
...###
####..
...#..
...#..
...#..
...#..
...#..
10 9 212
.......#.
.......#.
.......#.
#########
.......#.
.......#.
.......#.
.......#.
.......#.
.......#.
14 6 218
...#..
...#..
...#..
...#..
...#..
######
...#..
...#..
...#..
...#..
...#..
...#..
...#..
...#..
9 12 224
.....#......
.....#......
.....#......
.....#......
.....#......
.....#......
######......
.....##.....
......######
9 13 229
........#....
........#....
........#....
........#....
#############
.......#.....
.......#.....
.......#.....
.......#.....
10 13 235
.....#.......
.....#.......
.....#.......
#######......
......#......
......#######
......#......
......#......
......#......
......#......
```

### 输出 #1

```
164
1 26 6
1 25 6
1 24 6
1 23 6
1 22 6
1 21 6
1 20 6
1 19 6
1 18 6
1 17 6
1 16 6
1 15 6
1 14 6
1 13 6
1 13 5
1 13 4
1 1 0
1 1 1
1 1 2
1 1 3
1 1 4
1 2 4
1 3 4
1 4 4
1 5 4
1 6 4
1 7 4
1 8 4
1 9 4
1 10 4
1 11 4
1 12 4
1 0 25
1 0 26
1 0 27
1 0 28
1 0 29
1 0 30
1 0 31
1 0 32
1 0 33
1 0 34
1 0 35
1 0 36
1 0 37
1 0 38
1 0 39
1 0 40
1 0 41
1 0 42
1 0 43
1 41 9
1 40 9
1 39 9
1 38 9
1 37 9
1 36 9
1 35 9
1 34 9
1 33 9
1 32 9
1 31 9
1 30 9
1 29 9
1 28 9
1 27 9
1 26 9
1 26 8
1 26 7
1 1 32
1 2 32
1 3 32
1 4 32
1 5 32
1 6 32
1 7 32
1 8 32
1 9 32
1 10 32
1 11 32
1 12 32
1 49 21
1 48 21
1 47 21
1 46 21
1 45 21
1 44 21
1 43 21
1 42 21
1 41 21
1 41 20
1 41 19
1 41 18
1 41 17
1 41 16
1 41 15
1 41 14
1 41 13
1 41 12
1 41 11
1 41 10
1 40 21
1 39 21
1 38 21
1 38 22
1 38 23
1 38 24
1 38 25
1 38 26
1 38 27
1 38 28
1 38 29
1 38 30
1 38 31
1 38 32
1 38 33
1 0 24
1 0 23
1 0 22
1 0 21
1 0 20
1 0 19
1 0 18
1 0 17
1 0 16
1 0 15
1 0 14
1 0 13
1 0 12
1 0 11
1 0 10
1 0 9
1 0 8
1 0 7
1 0 6
1 0 5
1 0 4
1 49 49
1 48 49
1 47 49
1 46 49
1 45 49
1 44 49
1 43 49
1 42 49
1 41 49
1 40 49
1 39 49
1 38 49
1 38 48
1 38 47
1 38 46
1 38 45
1 38 44
1 38 43
1 38 42
1 38 41
1 38 40
1 38 39
1 38 38
1 38 37
1 38 36
1 38 35
1 38 34
```

## 说明/提示

### 测试用例数量

共 50 组

### 输入生成方法

固定参数：$ K=10 $，$ B=20 $。标记的坐标选自那些已经放置的标记，且必须保证选择的位置与所有现有标记的曼哈顿距离至少为 10。第一个标记在上边界（即 $ i_1=0 $ 处）随机选择，第二个标记在左边界（即 $ j_2=0 $ 处）随机选择，第三个在下边界（即 $ i_3=N-1 $ 处）随机选择，第四个则在右边界（即 $ j_4=N-1 $ 处）随机选择。

每个多连块用如下方法生成。一个多连块中包含的单元格称为**块**。第一个多连块包含 1 个块，成本为 $ C_1=50 $。对于第 $ b $ 个多连块，块数为 $ 2+b $，其成本计算为 $ C_b=\mathrm{round}(50\sqrt{2+b}) $。从 1 块的多连块开始，通过以下扩展操作进行 $ 1+b $ 次扩展：

1. 从上下左右四个方向中随机选取一个方向进行扩展。
2. 在该方向上选择最边缘的块，再将该方向上相邻的空位纳入多连块，从而扩展 1 个块。

### 工具

- [网页版可视化工具及输入生成器](https://img.atcoder.jp/future-fif-digital-days/visYp.html?q=b)
- [本地版可视化工具及输入生成器](https://img.atcoder.jp/future-fif-digital-days/dd7a70773bb74f0570cdde81b1bf6ee3.zip)：如需使用，请先安装 [Rust 语言](https://www.rust-lang.org/ja) 编译环境。

 **本翻译由 AI 自动生成**