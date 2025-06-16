## 题目描述
You are given a binary matrix $n \times n$ consisting of zeroes and ones. Initially, you have an empty string $S$. You start in the position $(0;0)$ (left-up corner) and move right or down. You append each element you have passed to the string $S$ in the respective order.

Tell whether it is possible to achieve $S$ being a palindrome. If yes, print the way it should pass to achieve that.

Note that each matrix is randomly generated.

## 输入格式
The first line contains the only integer $n$ $(1 \le n \le 5\,000)$ --- the size of a matrix.

The following $n$ lines contain the $n$ characters $a_{i,j}$ $(0 \le a_{i,j} \le 1)$ --- description of the matrix.

The input matrix for the problem is picked $\textbf{randomly}$ across all possible valid matrices for the problem of size $n \times n$.

## 输出格式
Print $\tt{NO}$ if there is no such palindrome. 

Otherwise, in the first line, print $\tt{YES}$. In each of the following $2n-1$ lines, print two integers $x_i$ and $y_i$ ($0 \leq x_i, y_i < n$) --- the coordinates of the $i$-th cell.

```input1
2
01
00
```

```output1
YES
0 0
0 1
1 1
```

```input2
4
0100
1010
0100
0001
```

```output2
NO
```

```input3
4
0010
1001
1010
0010
```

```output3
YES
0 0
0 1
0 2
0 3
1 3
2 3
3 3
```

## 提示
- ($5$ points) $n \le 10$;
- ($9$ points) $n \le 100$;
- ($19$ points) $n \le 500$;
- ($27$ points) $n \le 1\,500$;
- ($40$ points) no additional restrictions.

