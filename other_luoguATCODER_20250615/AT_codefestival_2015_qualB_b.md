# AT_codefestival_2015_qualB_b 採点

## 题目描述

题目大意：

高桥君正在编写一份试卷。很不幸的是，他忘记了一个题的正确答案。而他的N个学生用0~M之间的一个整数回答了这个问题。如果有超过一半的学生回答了一个整数X,那么高桥君就认定正确答案是这个整数X。
你会得到这N个学生的回答。如果高桥君打算以X为这道题的正解,那么请输出X。如果他无法以X为这道题的正解，那么请输出"?"（不包括外面的双引号）

## 输入格式

N M 
A1 A2 A3... AN
第一行是两个用空格隔开的整数N(1≤N≤10^5)和M（1≤M≤10^5）

第二行是用空格隔开的N个学生们的回答。保证每个学生的回答的整数不大于M 。

## 输出格式

如果高桥君认定正确答案为某个整数X，输出一个整数X。 否则，输出"?"。**务必在输出结束时输出换行符。**

## 输入输出样例 #1

### 输入 #1

```
3 2
2 1 2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4 2
2 1 2 1
```

### 输出 #2

```
?
```

## 输入输出样例 #3

### 输入 #3

```
10 1
0 0 0 0 0 0 1 1 1 1
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
10 5
0 1 2 3 4 5 5 5 5 5
```

### 输出 #4

```
?
```