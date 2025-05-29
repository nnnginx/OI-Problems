## Description

<div><p>Dr. TC has a new patient called Goblin. He wants to test Goblin's intelligence, but he has gotten bored of his standard test. So, he decided to make it a bit harder.</p><p>First, he creates a binary string$^{\text{∗}}$ $s$ having $n$ characters. Then, he creates $n$ binary strings $a_1, a_2, \ldots, a_n$. It is known that $a_i$ is created by first copying $s$, then flipping the $i$-th character ($\texttt{1}$ becomes $\texttt{0}$ and vice versa). After creating all $n$ strings, he arranges them into an $n \times n$ grid $g$ where $g_{i, j} = a_{i_j}$. </p><p>A set $S$ of size $k$ containing distinct integer pairs $\{(x_1, y_1), (x_2, y_2), \ldots, (x_k, y_k)\}$ is considered good if: </p><ul> <li> $1 \leq x_i, y_i \leq n$ for all $1 \leq i \leq k$. </li><li> $g_{x_i, y_i} = \texttt{0}$ for all $1 \leq i \leq k$. </li><li> For any two integers $i$ and $j$ ($1 \leq i, j \leq k$), coordinate $(x_i, y_i)$ is reachable from coordinate $(x_j, y_j)$ by traveling through a sequence of adjacent cells (which share a side) that all have a value of $\texttt{0}$. </li></ul><p>Goblin's task is to find the maximum possible size of a good set $S$. Because Dr. TC is generous, this time he gave him two seconds to find the answer instead of one. Goblin is not known for his honesty, so he has asked you to help him cheat.</p><div class="statement-footnote"><p>$^{\text{∗}}$A binary string is a string that only consists of characters $\texttt{1}$ and $\texttt{0}$.</p></div></div><div class="input-specification"><p>The first line of the input consists of a single integer $t$ $(1 \le t \le 10^3)$&nbsp;— the number of test cases.</p><p>The first line of each test contains a single integer $n$ $(1 \le n \le 2 \cdot 10^5)$&nbsp;— the length of the binary string $s$.</p><p>The second line of each test contains a single binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single number, the maximum possible size of a good set of cells from the grid.</p></div>

## Input

<p>The first line of the input consists of a single integer $t$ $(1 \le t \le 10^3)$&nbsp;— the number of test cases.</p><p>The first line of each test contains a single integer $n$ $(1 \le n \le 2 \cdot 10^5)$&nbsp;— the length of the binary string $s$.</p><p>The second line of each test contains a single binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single number, the maximum possible size of a good set of cells from the grid.</p>





```input1|2,3,6,7,10,11
6
3
000
4
0010
7
1011001
4
0001
2
11
1
0
```




```output1
3
9
10
7
1
0
```



## Note

<p>In the first example, the following grid has been written on the board:</p><p>$$ 1 0 0 $$ $$ 0 1 0 $$ $$ 0 0 1 $$</p><p>The set that consists of cells $(1, 2)$ and $(1, 3)$ is good. The set that consists of cells $(1, 1)$ and $(1, 2)$ is not good, since the value of cell $(1, 1)$ is not $0$. The set of cells $(1, 2)$, $(1, 3)$, $(2, 3)$ is good and has a maximum size of $3$. Note that the set of cells $(2, 1)$, $(3, 1)$, and $(3, 2)$ is also good with a maximum size of $3$.</p><p>In the second example, the following grid is written on the board:</p><p>$$ 1 0 1 0 $$ $$ 0 1 1 0 $$ $$ 0 0 0 0 $$ $$ 0 0 1 1 $$</p><p>And the maximum possible size of a good set is $9$.</p>
