# AT_relay2018_j 健康診断

## 题目描述

### 翻译题目
狼和狐狸要进行体检了。体检将持续一天，每只狼和狐狸将在一天中的某一时刻参加体检。第1天想参加体检的狼有$𝑤_{𝑖}$只，第1天想参加体检的狐狸有$f_{i}$只。
但是，在每天的每一时刻，只能诊断狼或狐狸中的一方。如果希望不一致的话，就要参加其他的时刻，但是如果想在第1时刻参加健康检查的狼和狐狸在第1时刻进行健康检查的话，不满度是$\lvert$i-j$\rvert$。不存在可以进行健康检查的时刻时，不满度为$10^{100}$。每只狼和狐狸都会在可以参加的其中不满程度最小的日子参加体检。
请在每天的每一时刻中，求出最适合诊断狼和狐狸时所有狼和狐狸的不满程度合计的最小值。

## 输入格式

第一行一个整数N，代表有N个时刻

接下来N行，每行两个数$w_{i}$，$f_{i}$

## 输出格式

一行，为不满度最小值

## 输入输出样例 #1

### 输入 #1

```
6
1 5
1 3
3 4
3 2
5 1
6 2
```

### 输出 #1

```
15
```

## 输入输出样例 #2

### 输入 #2

```
10
26 37
1 49
1 74
2 99
2 100
2 75
3 62
3 62
2 37
2 37
```

### 输出 #2

```
108
```