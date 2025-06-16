## 题目描述
In mathematics, the Fibonacci numbers, commonly denoted as $f_n$, is a sequence such that each number is the sum of the two preceding numbers, starting with $1$ and $1$. That is, $f_1 = 1, f_2 = 1$ and $f_n = f_{n-2} + f_{n-1}~(n \ge 3)$.

Thus, the beginning of the sequence is $1, 1, 2, 3, 5, 8, 13, 21,\ldots$ .

Given $n$, please calculate $\sum_{i=1}^{n}{\sum_{j=i+1}^{n}{g(f_i,f_j)}}$, where $g(x,y) = 1$ when $x \cdot y$ is even, otherwise $g(x,y) = 0$.

## 输入格式
The only line contains one integer $n~(1\le n\le 10^9)$.

## 输出格式
Output one number -- $\sum_{i=1}^{n}{\sum_{j=i+1}^{n}{g(f_i,f_j)}}$.

## 题目大意
在数学中，斐波拉契数列常被记为数列 $f_n$。该数列的首项 $f_1,f_2$ 均为 $1$，并满足递推公式 $f_n=f_{n-2}+f_{n-1}(n\ge 3)$。

因此，数列的前一些项为 $1,1,2,3,5,8,13,21,\cdots$。

若 $x\cdot y$ 为偶数，则函数 $g(x,y)=1$，否则 $g(x,y)=0$。求 $\sum\limits_{i=1}^n{\sum\limits_{j=i+1}^n{g(f_i,f_j)}}$ 的值。

```input1
3
```

```output1
2
```

```input2
10
```

```output2
24
```

```input3
100
```

```output3
2739
```

