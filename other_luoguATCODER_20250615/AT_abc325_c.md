# AT_abc325_c [ABC325C] Sensors

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc325/tasks/abc325_c

$ H $ 行 $ W $ 列のマス目の上に $ 0 $ 個以上のセンサが配置されています。上から $ i $ 行目、左から $ j $ 列目のマス目を $ (i,\ j) $ と表記します。   
 センサが配置されているマス目の情報は長さ $ W $ の文字列 $ S_1,\ S_2,\ \ldots,\ S_H $ によって与えられ、$ S_i $ の $ j $ 文字目が `#` のとき、またそのときに限り $ (i,\ j) $ にセンサが配置されています。  
 このセンサは上下左右斜めに隣接しているマス目に存在する他のセンサと連動し、一つのセンサとして動作します。 ただし、マス目 $ (x,\ y) $ と $ (x',\ y') $ が上下左右斜めに隣接しているとは、$ \max(|x-x'|,|y-y'|)\ =\ 1 $ であることを指します。  
 また、センサ $ A $ とセンサ $ B $ が連動し、センサ $ A $ とセンサ $ C $ が連動しているとき、センサ $ B $ とセンサ $ C $ も連動することに注意してください。

連動するセンサを一つのセンサと見なしたとき、このマス目の上にあるセンサの個数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_H $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 6
.##...
...#..
....##
#.#...
..#...
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3 3
#.#
.#.
#.#
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4 2
..
..
..
..
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
5 47
.#..#..#####..#...#..#####..#...#...###...#####
.#.#...#.......#.#...#......##..#..#...#..#....
.##....#####....#....#####..#.#.#..#......#####
.#.#...#........#....#......#..##..#...#..#....
.#..#..#####....#....#####..#...#...###...#####
```

### 输出 #4

```
7
```

## 说明/提示

### 制約

- $ 1\ \leq\ H,\ W\ \leq\ 1000 $
- $ H,\ W $ は整数
- $ S_i $ は各文字が `#` または `.` である長さ $ W $ の文字列
 
### Sample Explanation 1

連動しているセンサを一つのセンサと見なしたとき、 - $ (1,2),(1,3),(2,4),(3,5),(3,6) $ にあるセンサが連動したもの - $ (4,1) $ にあるセンサ - $ (4,3),(5,3) $ にあるセンサが連動したもの の $ 3 $ つのセンサが存在します。