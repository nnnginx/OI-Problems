## 题目描述
**This is an interactive problem.**

There are $n$ coins arranged in a row and numbered from $1$ to $n$ from left to right.

Exactly $k$ ($k<n$) of these coins are fake, and the other $(n-k)$ coins are real. The fake coins are lighter than the real ones. All real coins have the same weight, while fake coins may have different weights. It is also known that the fake coins are $\textbf{consecutive}$, that is, they have indexes $p, p+1, \dots, (p+k-1)$.

You need to find the number of the leftmost fake coin. You can use weighing, which is similar to weighing on a two-pan balance scale: select two sets of non-intersecting coins and find out which set weighs more, or that the sets weigh the same.

### Interactive Protocol

The first line contains three integers $n$, $k$, $g$ ($1 \le k < n \le 10^4$, $0 \le g \le 6$) - the total number of coins, the number of fake coins, and the test block number, respectively.

To perform the weighing request, output "$\texttt{?}$ $s_1$ $s_2$ $a_1$ $a_2$ $\dots$ $a_{s_1}$ $b_1$ $b_2$ $\dots$ $b_{s_2}$", where $s_1$ and $s_2$ denote the sizes of the sets being weighed, and the arrays $a$ and $b$ denote the numbers of the coins belonging to the first and second sets, respectively.

In response to the request, the jury program will output a single integer $x$ ($x \in \{0,1,2\}$). If $x = 1$, then the first set is heavier than the second; if $x = 2$, then the second set is heavier than the first; if $x = 0$, then the sets have the same weight.

If the request is invalid (i.e., the maximum number of requests has been exceeded or the request parameters are invalid), the jury program will output $\texttt{-1}$ and terminate. In this case, terminate your program to receive the verdict $\texttt{Wrong Answer}$.

Be sure to call the $\texttt{flush}$ method after outputting each line. You can use:
- $\texttt{fflush(stdout)}$, $\texttt{cout <{}< endl}$, or $\texttt{cout.flush()}$ in $\texttt{C++}$;
- $\texttt{System.out.flush()}$ in $\texttt{Java}$;
- $\texttt{flush(output)}$ in $\texttt{Pascal}$;
- $\texttt{sys.stdout.flush()}$ in $\texttt{Python}$;
- consult the documentation for other programming languages.
  
To give the answer, output a single line in the format "$\texttt{!}$ $p$", where $p$ ($1 \leq p \leq n$) is the number of the leftmost fake coin.

## 输入格式
See Interactive Protocol.

## 输出格式
See Interactive Protocol.

```input1
4 1 0

0

0

2
```

```output1

? 1 1 1 2

? 1 1 2 4

? 1 1 3 4

! 3
```

## 提示
Let's define $q$ as the maximum number of weighing queries you can make in the tests of a certain block.

- ($5$ points): $n \le 16$, $q=16$;
- ($9$ points): $k=1$, $q=16$;
- ($7$ points): $k=1$, $q=11$;
- ($16$ points): $k \le 16$, $q=11$;
- ($9$ points): all fake coins have the same weight, $q=11$;
- (up to $54$ points): $q=300$. Let the maximum number of weighings used be $c$. If $c \le 9$, you will get $54$ points, otherwise you will get $ \lfloor 54 \cdot \max(-0.0004 \cdot c + 0.3134, 0.018 + \frac{9.0773}{c}) \rfloor $ points.

Here is the $\tt{C++}$ code that computes the number of points for the last block of tests depending on the number of weighings used:

```cpp
((c <= 9) ? 54 : int(54 * (max((-0.0004 * c + 0.3134), (0.018 + 9.0773 / c)))))
```

### Scoring table

$$\begin{array}{|c|c|c|c|c|c|} 
\hline
c \leq 17 & \text{Points} & 18 \leq c \leq 27 & \text{Points} & 28 \leq c \leq 300 & \text{Points} \\
\hline
\leq 9 & 54 & 18 & 28 & 28 & 18 \\ 
10 & 49 & 19 & 26 & 29-30 & 17 \\ 
11 & 45 & 20 & 25 & 31-42 & 16 \\ 
12 & 41 & 21 & 24 & 43-89 & 15 \\ 
13 & 38 & 22 & 23 & 90-135 & 14 \\ 
14 & 35 & 23 & 22 & 136-181 & 13 \\ 
15 & 33 & 24 & 21 & 182-227 & 12 \\ 
16 & 31 & 25 & 20 & 228-274 & 11 \\ 
17 & 29 & 26-27 & 19 & 275-300 & 10 \\ 
\hline
\end{array}$$

