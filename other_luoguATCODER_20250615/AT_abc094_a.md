# AT_abc094_a [ABC094A] Cats and Dogs

## 题目描述

猫和狗一共有 $A+B$ 只，其中 $A$ 只是猫，剩下的 $B$ 只不知道是猫还是狗。

请判定这 $A+B$ 只猫和狗中，猫可能正好有 $X$ 只吗。

## 输入格式

输入以以下形式由标准输入给出。

$ A $ $ B $ $ X $

## 输出格式

如果猫正好有 $X$ 只的话就输出 $YES$ ，如果不可能的话就输出 $NO$ 。

## 输入输出样例 #1

### 输入 #1

```
3 5 4
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
2 2 6
```

### 输出 #2

```
NO
```

## 输入输出样例 #3

### 输入 #3

```
5 3 2
```

### 输出 #3

```
NO
```

## 说明/提示

限制:      
$1$ ≤ $A$ ≤ $100$  
$1$ ≤ $B$ ≤ $100$  
$1$ ≤ $X$ ≤ $200$  
输入为整数   
#### 样例 1   
$B$ = $5$ 只，如果猫 $1$ 只，狗 $4$ 只，则猫的数量合计为$X$ 只。

#### 样例 2 
即使两个不确定的都是猫，猫的数量合计也不足 $X$ 只。

#### 样例 2 
即使三个不确定的都是狗，猫的数量合计也会比 $X$ 只多。