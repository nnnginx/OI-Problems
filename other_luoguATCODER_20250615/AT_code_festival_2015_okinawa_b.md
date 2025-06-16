# AT_code_festival_2015_okinawa_b Beware of the Sogginess!

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2015-okinawa-open/tasks/code_festival_2015_okinawa_b

## 输入格式

Inputs will be given by standard input in following format.

> $ N $ $ X $ $ Y $ $ a_1 $ $ b_1 $ : $ a_N $ $ b_N $

- At the first line, integer $ N(1≦N≦50) $, $ X(1≦X≦10,000) $, $ Y(1≦Y≦10,000) $ will be given divided by spaces.
- From the second line there are $ N $ additional lines, for each line $ a_i\ (1≦\ a_i\ ≦10,000) $, $ b_i\ (1≦\ b_i\ ≦10,000) $ will be given divided by spaces.

## 输出格式

Please output the number of the minimum amount of items of Okinawa Soba that needs to be purchased to let Wolf Sothe to eat $ X $ or more than $ X $ grams of noodles and $ Y $ or more than $ Y $ grams of soup.

If there is no solution that meets Wolf Sothe’s need, output `-1`.

Print a newline at the end of output.

## 输入输出样例 #1

### 输入 #1

```
3 9 7
3 4
8 1
4 5
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5 20 24
8 1
4 6
10 3
10 2
5 10
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
5 6 8
1 3
6 2
2 3
3 5
1 4
```

### 输出 #3

```
3
```

## 说明/提示

### Problem

Hence Wolf Sothe likes eating Okinawa Soba (a kind of famous food in Okinawa, which is made of noodles and soup), he comes to an Okinawa Soba restaurant today. There are $ N $ different kinds of Okinawa Soba. At the beginning, the $ i_{th} $ kind of Okinawa Soba consists of $ a_i $ grams of noodles and $ b_i $ grams of soup.

Noodles will absorb soup after being purchased. Specifically, for the $ i_{th} $ kind of Okinawa Soba, if we had waited for $ t $ ($ t $ is a real number such that $ t≧0 $) seconds after the purchase, the weight of the noodles will be $ min(\ a_i\ +\ t\ ,\ a_i\ +\ b_i\ ) $ grams, the weight of soup will be $ max(\ b_i\ −\ t\ ,\ 0\ ) $ grams. The waiting time for each kind of Okinawa Soba is independent.

Wolf Sothe will choose a few kinds of Okinawa Soba among the $ N $ kinds to buy. For each kind of Okinawa Soba, there is only 1 item available.

Wolf Sothe wants to eat $ X $ or more than $ X $ grams of noodles and $ Y $ or more than $ Y $ grams of soup in total. Find the best solution that only needs the minimum amount of items of Okinawa Soba.

Please note that it costs no time for Wolf Sothe for eating Okinawa Soba, thus while Wolf Sothe is eating there is no absorption. In the other words, noodles will not absorb soup while Wolf Sothe is eating.

### Sample Explanation 1

Purchase the 1st and the 3rd kind of Okinawa Soba. For the 1st kind of Okinawa Soba, wait $ 2 $ second before eating. For the 3rd kind of Okinawa Soba, eat it as soon as it is purchased. Thus, it is possible to eat $ (3\ +\ 2)\ +\ (4\ +\ 0)\ =\ 9 $ grams of noodles and $ (4\ −\ 2)\ +\ (5\ −\ 0)\ =\ 7 $ grams of soup.

### Sample Explanation 2

Because there is less than $ 24 $ grams of soup in total, it is impossible to meet Wolf Sothe’s need even if all kinds of Okinawa Soba were purchased. Thus, output `-1`.