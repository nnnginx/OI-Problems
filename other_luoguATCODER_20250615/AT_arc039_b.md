# AT_arc039_b [ARC039B] 高橋幼稚園

## 题目描述

高桥先生是一名幼儿园老师。他决定给N个孩子发放K个糖果，每个孩子得到的糖果数都为整数个。
在这里，定义孩子们的整体幸福度为所有孩子得到的糖果的数量之乘积。
高桥先生发糖果时想尽量提高孩子们的整体幸福度，请你设计方案达到目的，并输出整体幸福度最高时的方案个数。（答案可能很大，请输出答案%1000000007的结果）
此题中，孩子们之间有差别，而糖果之间视为无差别。
** 请注意有孩子未分到糖果时乘积为零的情况（详见样例三）**

## 输入格式

保证由以下格式输入：
一行，两个正整数N(1<=N<=100)和K(1<=K<=500)（含义见描述），由空格隔开。

## 输出格式

一个数，即答案mod 1000000007的结果，并附加一个换行符。
# 输入输出样例
### 输入样例#1：
```
4 10
```
### 输出样例#1：
```
6
```
### 输入样例#2：
```
100 450
```
### 输出样例#2：
```
538992043
```
### 输入样例#3：
```
5 2
```
### 输出样例#3：
```
15
```

## 输入输出样例 #1

### 输入 #1

```
4 10
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
100 450
```

### 输出 #2

```
538992043
```

## 输入输出样例 #3

### 输入 #3

```
5 2
```

### 输出 #3

```
15
```

## 说明/提示

### **数据范围**
- 有80%数据满足N<=K
### **样例说明1**
这四个孩子中有两个人分到2颗糖果，两个人分到3颗糖果时整体幸福度最大，最大值为2×2×3×3=36.
分配方式有(3,3,2,2),(3,2,3,2),(3,2,2,3),(2,3,3,2),(2,3,2,3),(2,2,3,3) 共6种.
### **样例说明2**
注意答案取模1000000007
### **样例说明3**
无论你如何分发糖果，整体幸福度都为0。