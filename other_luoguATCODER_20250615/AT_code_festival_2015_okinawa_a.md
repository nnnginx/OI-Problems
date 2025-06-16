# AT_code_festival_2015_okinawa_a Automatic Map Generator

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-okinawa-open/tasks/code_festival_2015_okinawa_a

## 输入格式

Inputs will be given by standard input in following format

> $ H $ $ W $ $ K $

- At the first line, $ H\ (1\ ≦\ H\ ≦\ 100) $ 、 $ W\ (1\ ≦\ W\ ≦\ 100) $ 、 $ K\ (1\ ≦\ K\ ≦\ 10,000) $ will be given divided by spaces.

## 输出格式

Output `IMPOSSIBLE` if it is impossible to draw exactly $ K $ islands. Otherwise, output $ H $ lines where the $ i_{th} $ line has $ W $ letters, and the $ j_{th} $ letter from the left side of the $ i_{th} $ line must be the letter that Cat Snuke draws on her paper.

If there are multiple possible solutions, it is allowed to output any of them.

Print a newline at the end of output.

## 输入输出样例 #1

### 输入 #1

```
6 7 4
```

### 输出 #1

```
#.#####
..#...#
#.#.#.#
#.#...#
#..####
.#..###
```

## 输入输出样例 #2

### 输入 #2

```
2 4 3
```

### 输出 #2

```
IMPOSSIBLE
```

## 输入输出样例 #3

### 输入 #3

```
20 50 10
```

### 输出 #3

```
..................................................
...........................................#......
..........................................#.......
..................................................
..........................................#.......
..............................................#...
.....................................##..#....##..
.........................................##..###..
..........................#...............#####...
..........................................####....
.........................................###......
......##...............#..............#.#.........
.......##.............................##..........
........#.............................###.........
.....................................##...........
.............................#.......##...........
.............................#..#.................
...........................#....#.................
..................................................
..................................................
```

## 说明/提示

### Problem

As is known to all, Okinawa is comprised of various islands. Cat Snuke wants to draw a simple map to include some of these islands. However, since the size of the paper is limited, Snuke will not be able to draw the map in details.

Therefore, Cat Snuke divides the paper into grids, which have $ H $ horizontal rows and $ W $ vertical columns. For each block of the grids, it will be filled with either a `.` that represents the sea or a `#` that represents the land.

Each island consists of blocks of land. For two blocks that represent land, we say that they belong to the same island, only if they had coincident edges or vertexes, or they were connected by other blocks that have coincident edges or vertexes. Otherwise, we say these two blocks belong to different islands.

Suppose that there is only sea beyond Snuke’s map. Also, please note that the blocks of land that is surrounded by sea that is surrounded by an island belong to another island (rather than the outer island).

Cat Snuke needs to follow the rules above to draw exactly $ K $ islands on the paper. Please decide whether Snuke is able to draw. If your answer was yes, please find a solution.

### Sample Explanation 1

There are four islands. Although the land block at the 3rd row from the top and the 5th column from the left is surrounded by an outer island, they are separated because that there is sea between them and they share no edges nor vertices.

### Sample Explanation 2

The paper is too small to draw a map that satisfies the conditions.