# AT_jag2018summer_day2_a 10^N+7

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2018summer-day2/tasks/jag2018summer_day2_a

有三个非负整数 $ x,y,z $，你需要找到符合以下条件的最小非负整数 $n$ :

- $ n\ {\rm\ mod}\ 17\ =\ x $
- $ n\ {\rm\ mod}\ 107\ =\ y $
- $ n\ {\rm\ mod}\ 1000000007(=10^9+7)\ =\ z $

## 输入格式

输入三个非负整数 $x,y,z$（用空格隔开）

## 输出格式

输出符合要求的 $n$ 的最小值

## 输入输出样例 #1

### 输入 #1

```
15 50 1
```

### 输出 #1

```
1000000008
```

## 输入输出样例 #2

### 输入 #2

```
0 0 0
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
3 14 159265358
```

### 输出 #3

```
1050159272708
```

## 说明/提示

- $ 0\ \leq\ x\ <\ 17 $
- $ 0\ \leq\ y\ <\ 107 $
- $ 0\ \leq\ z\ <\ 10^9+7 $