# AT_abc378_b [ABC378B] Garbage Collection

## 题目描述

### 题目翻译

在 AtCoder 市，有 $ N $ 种垃圾会被定期收集。第 $ i\;(i = 1, 2, \dots, N) $ 种垃圾会在日期对 $ q_i $ 取余后等于 $ r_i $ 的日子被收集。

请回答 $ Q $ 个问题。对于第 $ j\;(j = 1, 2, \dots, Q) $ 个问题，若第 $ t_j $ 种垃圾在第 $ d_j $ 日产生，求该垃圾会在什么时候被收集。

如果在产生垃圾的当天，恰好是该种垃圾被收集的日子，则可以在同一天收集。

## 输入格式

输入从标准输入读取，格式如下：

> $ N $  
> $ q_1 $  $ r_1 $  
> $ q_2 $  $ r_2 $  
> $ \vdots $  
> $ q_N $  $ r_N $  
> $ Q $  
> $ t_1 $ $ d_1 $  
> $ t_2 $ $ d_2 $  
> $ \vdots $  
> $ t_Q $ $ d_Q $

## 输出格式

输出 $ Q $ 行。第 $ j\;(1 \leq j \leq Q) $ 行应为第 $ j $ 个问题的答案。

### 数据限制

- $ 1 \leq N \leq 100 $
- $ 0 \leq r_i < q_i \leq 10^9 $
- $ 1 \leq Q \leq 100 $
- $ 1 \leq t_j \leq N $
- $ 1 \leq d_j \leq 10^9 $
- 输入的所有数值均为整数

### 对样例 1 的解释

- 对于第 $ 1 $ 个问题：第 $ 1 $ 种垃圾在第 $ 1 $ 天产生，之后在第 $ 3 $ 天被收集。
- 对于第 $ 2 $ 个问题：第 $ 1 $ 种垃圾在第 $ 3 $ 天产生，之后在第 $ 3 $ 天被收集。
- 对于第 $ 3 $ 个问题：第 $ 1 $ 种垃圾在第 $ 4 $ 天产生，之后在第 $ 10 $ 天被收集。

## 输入输出样例 #1

### 输入 #1

```
2
7 3
4 2
5
1 1
1 3
1 4
1 15
2 7
```

### 输出 #1

```
3
3
10
17
10
```