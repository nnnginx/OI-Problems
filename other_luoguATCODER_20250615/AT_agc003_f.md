# AT_agc003_f [AGC003F] Fraction of Fractal

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc003/tasks/agc003_f

高橋君はお母さんからグリッドをもらいました。このグリッドは縦 $ H $ マス×横 $ W $ マスからなり、各マスは黒か白で塗られています。 黒いマス全体は、縦横にひとつながりになっています。

このグリッドの $ i $ 行 $ j $ 列 $ (1\ ≦\ i\ ≦\ H,\ 1\ ≦\ j\ ≦\ W) $ のマスの情報は、縦横に並んだ文字 $ s_{ij} $ であらわされ、 $ s_{ij} $ が `#` のときこのマスが黒く、 `.` のとき白く塗られていることを表します。少なくともひとつのマスが黒く塗られています。

レベル $ 0 $ のフラクタルとは黒いマスひとつからなる $ 1\ ×\ 1 $ のグリッドであり、 レベル $ k+1 $ のフラクタルとは、レベル $ k $ のフラクタルを、お母さんからもらったグリッドの全ての黒いマスに相当する位置に並べ、白いマスに相当する位置は白いマスで埋めたものを指します。

お母さんからもらったグリッドの情報と整数 $ K $ が与えられるので、レベル $ K $ のフラクタルに黒いマスからなる連結成分がいくつあるかを $ 10^9+7 $ で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ K $ $ s_{11}\ ..\ s_{1W} $ : $ s_{H1}\ ..\ s_{HW} $

## 输出格式

レベル $ K $ のフラクタルにある黒いマスからなる連結成分の個数を $ 10^9+7 $ で割ったあまりを一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3 3
.#.
###
#.#
```

### 输出 #1

```
20
```

## 输入输出样例 #2

### 输入 #2

```
3 3 3
###
#.#
###
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
11 15 1000000000000000000
.....#.........
....###........
....####.......
...######......
...#######.....
..##.###.##....
..##########...
.###.....####..
.####...######.
###############
#.##..##..##..#
```

### 输出 #3

```
301811921
```

## 说明/提示

### 制約

- $ 1\ ≦\ H,W\ ≦\ 1000 $
- $ 0\ ≦\ K\ ≦\ 10^{18} $
- $ s_{ij} $ は `#` か `.` のいずれかである。
- `#` のマス全体は縦横に連結である。
- `#` のマスは少なくともひとつ存在する。

### Sample Explanation 1

この入力例で作られるフラクタルは、以下のようなものです。この黒マスからなる連結成分の数は $ 20 $ なので、$ 20 $ を出力します。 ``` .............#............. ............###............ ............#.#............ ..........#..#..#.......... .........#########......... .........#.##.##.#......... ..........#.....#.......... .........###...###......... .........#.#...#.#......... ....#........#........#.... ...###......###......###... ...#.#......#.#......#.#... .#..#..#..#..#..#..#..#..#. ########################### #.##.##.##.##.##.##.##.##.# .#.....#..#.....#..#.....#. ###...######...######...### #.#...#.##.#...#.##.#...#.# ....#.................#.... ...###...............###... ...#.#...............#.#... .#..#..#...........#..#..#. #########.........######### #.##.##.#.........#.##.##.# .#.....#...........#.....#. ###...###.........###...### #.#...#.#.........#.#...#.# ```