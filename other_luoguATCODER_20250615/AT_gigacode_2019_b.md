# AT_gigacode_2019_b 採用面接

## 题目描述

某公司要进行面试，面试的能力有两项：「技术值」「社交值」。  
满足以下条件的人视为面试合格

- 技术值大于等于 $X$，社交值大于等于 $Y$。
- 技术值和社交值的总和大于等于 $Z$。  

有 $N$ 个人来面试，第 $i$ 个人技术值为 $A_i$，社交值为 $B_i$。请求出一共有多少人面试合格。

## 输入格式

第一行输入三个整数 $N,X,Y,Z$。  
接下来 $N$ 行，每行输入两个整数 $A_i,B_i$。

## 输出格式

输出一个整数，表示有多少人面试合格。

## 输入输出样例 #1

### 输入 #1

```
1 60 20 100
72 28
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
5 70 70 150
72 77
70 90
65 88
75 75
97 84
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
15 80 60 150
20 24
33 17
29 36
40 18
15 27
10 41
53 77
42 15
12 17
32 10
19 28
37 27
91 2
13 25
40 40
```

### 输出 #3

```
0
```