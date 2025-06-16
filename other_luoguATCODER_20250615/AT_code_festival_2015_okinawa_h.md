# AT_code_festival_2015_okinawa_h Happy 2015

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-okinawa-open/tasks/code_festival_2015_okinawa_h

## 输入格式

Inputs will be given by standard input in following format

> $ N $ $ l_1 $ $ r_1 $ $ l_2 $ $ r_2 $ : $ l_N $ $ r_N $

- At the first line, an integer $ N(1≦N≦2,000) $ will be given divided by a space.
- From the second line there are $ N $ additional lines to give the information about the illumination range. For the $ i_{th} $ line, integer $ l_i $, $ r_i(0≦l_i\ <\ r_i≦1,000,000,000) $ will be given divided by a space.

## 输出格式

Please answer the number of the different illumination combinations, modulo $ 1,000,000,007 $.

Print a newline at the end of output.

## 输入输出样例 #1

### 输入 #1

```
4
0 1
1 2
0 2
1 3
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
12
0 4
7 12
1 3
6 8
2 3
4 6
8 9
2 7
9 11
1 2
3 5
7 9
```

### 输出 #2

```
240
```

## 输入输出样例 #3

### 输入 #3

```
14
0 1
2 3
4 5
6 7
8 9
10 11
12 13
14 15
16 17
18 19
0 3
4 7
8 13
14 19
```

### 输出 #3

```
2025
```

## 说明/提示

### Problem

As the end of year $ 2015 $ approaching, the downtown area has been lighted up to celebrate year’s end. At this year, Cat Snuke also enjoys making a light-up device for the downtown area.

The downtown can be regarded as a one-dimensional line of numbers. There are $ N $ lights that have been installed on this number line. When the power of the $ i_{th} $ light is on, it can illuminate an interval of $ [l_i,\ r_i] $ (inclusive).

Although Cat Snuke can switch on the $ N $ lights independently as his wish, he wants to try different illumination combinations as many as possible. Then, if we had tried all the combinations of $ 2^N $ illumination combinations, we want to know how many different illumination combinations there are, of which each combination is a set of points that for each point in it can be illuminated by one or more lights.

When we tried all the $ 2^N $ illumination combination, please answer the number of the different illumination combinations, modulo $ 1,000,000,007 $.

### Sample Explanation 1

There are $ 16 $ different ways of attaching the light power, but there are only $ 6 $ different illumination combinations, $ \{φ\},\ \{[0,\ 1]\},\ \{[1,\ 2]\},\ \{[0,\ 2]\},\ \{[1,\ 3]\},\ \{[0,\ 3]\} $.