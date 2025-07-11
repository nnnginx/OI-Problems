# AT_abc356_c [ABC356C] Keys

## 题目描述

你有 $N$ 个编号为 $1, 2, \dots, N$ 的密钥。  
其中一些是真钥匙，其他都是假钥匙。

有一扇 X 门，你可以插入任意数量的钥匙。只有插入至少 $K$ 把真钥匙，X 门才会打开。

你已经对这些钥匙进行了 $M$ 次测试。第 $i$ 次测试过程如下：

- 您将 $C_i$ 把 $A_{i,1}, A_{i,2}, \dots, A_{i,C_i}$ 把钥匙插入了 X 门。
- 测试结果用一个英文字母 $R_i$ 表示。
    - $R_i =$ o "表示在第 $i$ 次测试中，X 门打开了。
    - $R_i =$ x "表示在第 $i$ 次测试中，X 门没有打开。

有 $2^N$ 种可能的钥匙组合，其中哪些是真钥匙，哪些是假钥匙。在这些组合中，找出与任何测试结果都不矛盾的组合数。  
给定的测试结果有可能是错误的，没有任何组合满足条件。在这种情况下，报告 $0$ 。

## 输入格式

#### 输入

输入内容由标准输入法提供，格式如下

>$N$ $M$ $K$
>
>$C_1$ $A_{1,1}$ $A_{1,2}$ $\dots$ 
>
>$A_{1,C_1}$ $R_1$
>
>$C_2$ $A_{2,1}$ $A_{2,2}$ $\dots$ 
>
>$A_{2,C_2}$ $R_2$
>
>$\vdots$
>
>$C_M$ $A_{M,1}$ $A_{M,2}$ $\dots$ 
>
>$A_{M,C_M}$ $R_M$

## 输出格式

将答案输出为整数。

## 输入输出样例 #1

### 输入 #1

```
3 2 2
3 1 2 3 o
2 2 3 x
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4 5 3
3 1 2 3 o
3 2 3 4 o
3 3 4 1 o
3 4 1 2 o
4 1 2 3 4 x
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
11 4 9
10 1 2 3 4 5 6 7 8 9 10 o
11 1 2 3 4 5 6 7 8 9 10 11 o
10 11 10 9 8 7 6 5 4 3 2 x
10 11 9 1 4 3 7 5 6 2 10 x
```

### 输出 #3

```
8
```

## 说明/提示

#### 限制因素

- $N$ 、 $M$ 、 $K$ 、 $C_i$ 和 $A_{i,j}$ 为整数。
- $1 \le K \le N \le 15$
- $1 \le M \le 100$
- $1 \le C_i \le N$
- $1 \le A_{i,j} \le N$
- $A_{i,j} \neq A_{i,k}$ 如果 $j \neq k$ .
- $R_i$ 是 `o` 或 `x`。

#### 样例 $1$ 说明

在此输入中，有三个键，进行了两次测试。  
打开 X 门需要两把正确的钥匙。

- 在第一次测试中，使用了钥匙 $1, 2, 3$ ，X 门打开了。
- 在第二次测试中，使用了钥匙 $2, 3$ ，X 门没有打开。

有两种组合，哪把钥匙是真钥匙，哪把钥匙是假钥匙，测试结果都没有矛盾：

- 钥匙 $1$ 是真的，钥匙 $2$ 是假的，钥匙 $3$ 是真的。
- 密钥 $1$ 是真实的，密钥 $2$ 是真实的，密钥 $3$ 是假的。

#### 样例 $2$ 说明

如问题陈述所述，答案可能是 $0$ 。