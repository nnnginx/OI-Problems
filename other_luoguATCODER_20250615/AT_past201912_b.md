# AT_past201912_b 増減管理

## 题目描述

某商品的 $N$ 天销售额为整数列 $A_1, A_2,... , A_N$ 。$A_i（1 \le i\le N）$ 表示第 $i$ 天的销售额。

你决定制作一个从第 $2$ 天开始，以后的每一天输出当天的销售额比前一天的销售额高多少（或者低）的程序。

更具体地说，程序输出 $N-1$ 行，第 $i$ 行（$ 1≤i≤N-1$ ）的内容如下：

-  $A_{i+1} = A_i$ ，输出 `stay` 。

- $ A_{i+1} < A_i$ ，输出 `down[减少量]` ，其中 `[减少量]` 为整数值 $A_i-A_{i+1}$ 。

- $ A_{i+1} > A_i$ ，输出 `up[增量]` ，其中 `[增量]` 为整数值 $A_{i+1}- A_i$ 。

请你制作这个程序。

## 输入格式

输入一个整数 $N$ 。

接下来 $N$ 行，每行输入一个整数 $a_i$ 。

## 输出格式

按照问题中的指示输出N-1行。

## 输入输出样例

### 输入 #1

```
10
9
10
3
100
100
90
80
10
30
10
```

### 输出#1

```
up 1
down 7
up 97
stay
down 10
down 10
down 70
up 20
down 20
```

## 输入输出样例 #1

### 输入 #1

```
10
9
10
3
100
100
90
80
10
30
10
```

### 输出 #1

```
up 1
down 7
up 97
stay
down 10
down 10
down 70
up 20
down 20
```

## 说明/提示

$2 \le N \le 100,000$

$0 \le A_i \le 1,000,000,000$

by @[NOI_AK_dreeeam](https://www.luogu.com.cn/user/686445)