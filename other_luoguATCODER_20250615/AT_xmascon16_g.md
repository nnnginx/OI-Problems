# AT_xmascon16_g Guide Passengers

## 题目描述

## 题目意思  
兔子铁路是兔子专用的铁路。车站从西到右依次编号为1～N（1≤i≤N）。各站都有限制C，车站只能同时有Ci只兔子等车。  
铁道计划运行M（1≤i≤M）趟列车，列车是在时刻Si从车站Ai出发，在时刻Ti到达车Ai+1，只可以搭载兔子Bi只。  
现在，车站1有一只C1的兔子，所有兔子都想去车站N，最多能搬运几只兔子到车站N？  

## 样例1解释   
可以像以下那样搬运5只兔子。  
-列车1乘坐3只。  
-在车站2全体换乘列车2（到站时另一辆列车--2号车恰好来了，所以不考虑车站2的限制。  
-在车站3全体下车。  
-列车4乘坐5只。  
-在车站2全体下车等待列车3（3号车还没到，所以要等车，考虑限制为C2--2只兔子，所以5只兔子只留了2只等车，剩下的可以不用运过来，放回车站1）。  
-剩下的两只乘坐列车3。  
-在车站3全体下车。  
共计5只兔子来到n站。

## 输入格式

第一行两个整数 $N$ $M$，表示车站数和列车数。  
第二行$N$个整数 $C1...Cn$ ,表示每个车站的限制。   
接下来$M$组数据：  
$S,T,A,B$。

## 输出格式

一个整数$N$,到n站的兔子数。

## 输入输出样例 #1

### 输入 #1

```
3 4
9 2 9
1 2 1 3
2 3 2 4
6 9 2 5
2 4 1 5
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
3 2
1 9 9
1 2 1 5
3 4 2 5
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
2 1
1000000000 2016
999999999 1000000000 1 1000000000
```

### 输出 #3

```
2016
```

## 输入输出样例 #4

### 输入 #4

```
2 0
12 24
```

### 输出 #4

```
0
```

## 输入输出样例 #5

### 输入 #5

```
4 11
8 2 3 9
1 2 1 1
2 4 1 1
4 5 1 6
6 7 1 1
6 7 2 3
5 6 2 5
3 4 2 3
4 6 3 2
6 7 3 1
7 8 3 4
8 9 3 2
```

### 输出 #5

```
7
```