## 题目描述
Givena $n×n$ matrix $A$ and apositive integer $k$，find the sum $S=A+A^2 +A^3 +...+A^k$.

## 输入格式
The input contains exactly one test case. The first line of input contains three positive integers $n$ ($n \le 30$), $k$ ($k \le 10^9$) and $m$ ($m < 10^4$). Then follow n lines each containing $n$ non negative integers below 32,768, giving $A$’s elements in row-major order.

## 输出格式
Output the elements of $S$ modulo $m$ in the same way as $A$ is given.

## 题目大意
**【题目描述】**

给定一个 $n×n$ 矩阵 $A$ 和一个正整数 $k$，找出和 $S=A+A^2 +A^3 +...+A^k$。

**【输入格式】**

输入包含一个测试用例。输入的第一行包含三个正整数 $n$（$n \le 30$）、$k$（$k \le 10^9$）和 $m$（$m < 10^4$）。接下来的 $n$ 行每行包含 $n$ 个小于 32,768 的非负整数，按行主序给出 $A$ 的元素。

**【输出格式】**

以与给定 $A$ 相同的方式输出 $S$ 的元素对 $m$ 取模。

翻译来自于：[ChatGPT](https://chatgpt.com/)

```input1
2 2 4 
0 1 
1 1
```

```output1
1 2
2 3
```

