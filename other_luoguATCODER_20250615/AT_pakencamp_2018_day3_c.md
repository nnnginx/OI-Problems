# AT_pakencamp_2018_day3_c 竹の観察

## 题目描述

### 题目简述

开始时，有一个正整数 $a$。每次迭代是指将 $a$ 变为 $\lfloor\frac{3}{2}a\rfloor$（$\lfloor x\rfloor$ 表示将 $x$ 下取整）。已知 $a$ 经过若干次 **（至少一次）** 迭代后得到了 $b$，请求出 $a$ 有多少种可能的取值。

## 输入格式

一行一个整数 $b$。

## 输出格式

一行一个整数，$a$ 的可能取值个数。**建议在输出末尾添加换行。**

## 输入输出样例 #1

### 输入 #1

```
10
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8092
```

### 输出 #3

```
21
```

## 输入输出样例 #4

### 输入 #4

```
3687
```

### 输出 #4

```
12
```

## 说明/提示

#### 样例 #3 说明

当 $b=8092$ 时，答案最大，为 $21$。

#### 数据规模与约定

**本题设有子任务。**  
**子任务 1（30 pts）：** $b\le 10$。  
**子任务 2（70 pts）：** 无追加限制。

对于全部测试数据，都有 $2\le b\le 10000$。