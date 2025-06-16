## 题目描述
Given an array $a$ consisting of $n$ integers. For one operation, you can choose position $i$ ($1 \leq i \leq n$), decrease $a_i$ by $k$, and increase the value of all other elements $a_j$ ($1 \leq j \leq n, i \neq j$) by $t$.

Find the minimum number of operations needed to make all elements of the array less than or equal to zero (i.e., non-positive), or report that it is impossible to do so.

## 输入格式
The first line contains three integers $n$, $k$, $t$ ($1 \leq n \leq 10^6$, $0 \leq k, t \leq 10^9$) --- the length of the array and the operation parameters.

The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^{18} \leq a_i \leq 10^9$) --- the initial values of the array elements.

## 输出格式
Output a single integer $c$ --- the minimum number of operations needed to make all elements of the array less than or equal to zero. If it is impossible, output $-1$.

If it is possible, output $n$ integers $cnt_i$ ($1 \leq i \leq n$), which represent the number of operations performed on the element with index $i$. Note that the equality $\sum\limits_{i=1}^n cnt_i = c$ must hold.

```input1
4 10 1
2 5 9 -4
```

```output1
4
1 1 2 0 
```

```input2
5 1 100
-1000 -1000 10 -1000 -1000
```

```output2
10
0 0 10 0 0 
```

```input3
2 1 1
1 0
```

```output3
-1
```

## 提示
- ($3$ points) $t = 0$;
- ($5$ points) $1 \leq n \leq 300, 0 \leq |a_i| \leq 300, 0 \leq t \leq 10^6$;
- ($8$ points) $1 \leq n \leq 3000, 0 \leq |a_i| \leq 3000, 0 \leq t \leq 10^6$;
- ($9$ points) $1 \leq n \leq 10^3, 1 \leq a_i \leq 10^9, 0 \leq t \leq 10^6$;
- ($5$ points) $1 \leq n \leq 10^4, 1 \leq a_i \leq 10^9$;
- ($13$ points) $1 \leq n \leq 10^5, 1 \leq a_i \leq 10^9$;
- ($8$ points) $1 \leq a_i \leq 10^9$;
- ($9$ points) $1 \leq n \leq 10^3, 0 \leq t \leq 10^6$;
- ($5$ points) $1 \leq n \leq 10^4$;
- ($14$ points) $1 \leq n \leq 10^5$;
- ($21$ points) without additional constraints.

