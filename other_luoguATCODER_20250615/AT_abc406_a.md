# AT_abc406_a 不可接受

## 题目描述

高桥先生在 $2025$ 年 $5$ 月 $17$ 日 $A$ 时 $B$ 分截止的报告中，于 $2025$ 年 $5$ 月 $17$ 日 $C$ 时 $D$ 分提交。  
确保 $A$ 时 $B$ 分和 $C$ 时 $D$ 分 是不同的时间。

如果高桥先生在截止前提交了报告，则输出 `Yes`；否则输出 `No`。

## 输入格式

输入将以以下格式从标准输入中给出。

> $A\ B\ C\ D$

## 输出格式

如果高桥先生在截止前提交了报告，则输出 `Yes`；否则输出 `No`。

## 输入输出样例 #1

### 输入 #1

```
22 40 22 30
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
22 40 22 45
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
12 0 11 30
```

### 输出 #3

```
Yes
```

## 说明/提示

### 约束
- $0 \leq A, C \leq 23$
- $0 \leq B, D \leq 59$
- $(A, B) \neq (C, D)$
- $A, B, C, D\isin \mathbb Z$
### 样例 1 解释
报告的截止时间是 $22$ 时 $40$ 分，高桥君在 $22$ 时 $30$ 分提交，因此他在截止日期前提交了报告。  
因此，输出 `Yes`。
### 样例 2 解释
报告的截止时间是 $22$ 时 $40$ 分，高桥君在 $22$ 时 $45$ 分提交，因此是在截止时间后提交报告。  
因此，输出 `No`。