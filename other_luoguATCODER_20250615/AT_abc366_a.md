# AT_abc366_a [ABC366A] Election 2

## 题目描述

### 问题陈述
AtCoder 市正在举行市长选举。候选人是高桥和青木。

有 N 张有效选票投给两位候选人中的任何一位，目前正在进行计票。 N 是奇数。

目前的计票结果是：高桥 
T 票，青木 
A 票。

请判断此时选举结果是否已经确定。
### 限制因素

- $1 \leq N \leq 99$
- $N$ 是奇数。
- $0 \leq T, A \leq N$
- $T + A \leq N$
- 所有输入值均为整数。

## 输入格式

N A T

## 输出格式

如果选举结果已经确定，则打印 "Yes"，否则打印 "No"。
### 样本输出1解释

即使剩下的一票投给青木，高桥仍将获胜。也就是说，他的胜负已定，所以打印 "Yes"。
### 样本输出2解释
虽然青木目前的票数更多，但如果高桥获得剩余的 $39$ 票，他就会获胜。因此，打印 "No"。

## 输入输出样例 #1

### 输入 #1

```
7 4 2
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
99 12 48
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
1 0 0
```

### 输出 #3

```
No
```