## 题目描述

有 $n$ 个二元组 $(a_i,~b_i)$，编号为 $1$ 到 $n$。

有一个初始为空的栈 $S$ ，向其中加入元素 $(a_i,~b_i)$ 时，先不断弹出栈顶元素直至栈空或栈顶元素 $(a_j,~b_j)$ 满足 $a_i \ne a_j$ 且 $b_i \le b_j$，然后再将其加入栈中。

如果一个二元组入栈后栈内只有这一个元素，则称该二元组是“成功的”。

有 $q$ 个询问 $[l_i,~r_i]$ ，表示若将编号在 $[l_i,~r_i]$ 中的二元组按编号从小到大依次入栈，会有多少个二元组是“成功的”。

询问之间相互独立。

## 输入格式

第一行两个正整数 $n$，$q$。  
第二行 $n$ 个正整数表示 $a_i$。  
第三行 $n$ 个正整数表示 $b_i$。  
接下来 $q$ 行，每行两个正整数 $l_i,~r_i$, 表示一组询问。

## 输出格式

$q$ 行，每行一个自然数表示一组询问的答案。

```input1
10 4
3 1 3 1 2 3 3 2 1 1
10 10 2 9 7 5 4 7 6 1
1 4
7 8
7 10
1 8
```
```output1
3
2
2
3
```

## 样例解释

以第一次询问 $[1,~4]$ 为例。

一开始栈为 $\{\}$。  
加入 $1$ 号二元组后栈为 $\{(3,~10)\}$ ，栈中只有一个元素，该二元组是“成功的”。  
加入 $2$ 号二元组 $(1,~10)$ 时，栈顶的 $(3,~10)$ 的 $b$ 值不大于 $2$ 号二元组的，因此弹栈。此时栈空，$2$ 号二元组入栈，栈为 $\{(1,~10)\}$ ，该二元组是“成功的”。  
加入 $3$ 号二元组 $(3,~2)$ ，此时栈顶元素与之 $a$ 值不同，$b$ 值比它更大，因而不需要弹栈，直接将 $3$ 号二元组入栈，栈为 $\{(1,~10), (3,~2)\}$ ，栈中有多个元素，该二元组不是“成功的”。  
加入 $4$ 号二元组 $(1,~9)$ ，此时栈顶元素 $(3,~2)$ 的 $b$ 值比它小，弹栈。弹栈后栈顶元素 $(1,~10)$ 与 $(1,~9)$ 的 $a$ 值相同，继续弹栈。此时栈空，$4$ 号二元组入栈，栈为 $\{(1,~9)\}$，该二元组是“成功的”。

共有 $3$ 个二元组是“成功的”，因而答案为 $3$。

## 输入输出数据 2

见 [`stack2.in`](./5166/file/stack2.in) 与 [`stack2.ans`](./5166/file/stack2.ans)。

## 输入输出数据 3

见 [`stack3.in`](./5166/file/stack3.in) 与 [`stack3.ans`](./5166/file/stack3.ans)。

## 输入输出数据 4

见 [`stack4.in`](./5166/file/stack4.in) 与 [`stack4.ans`](./5166/file/stack4.ans)。

## 数据范围与提示

对于所有测试点：$1 \le n, q \le 5 \times 10^5$，$1 \le a_i, b_i \le n$，$1 \le l_i \le r_i \le n$。

每个测试点的具体限制见下表：

|  测试点编号  |    特殊性质     |
| :----------: | :-------------: |
|  $1 \sim 3$  | $n,q \leq 1000$ |
|  $4 \sim 6$  |  $n \leq 5000$  |
| $7 \sim 10$  | $n,q \leq 10^5$ |
| $11 \sim 12$ |   $b_i=n-i+1$   |
| $13 \sim 15$ |     $a_i=i$     |
| $16 \sim 20$ |       无        |