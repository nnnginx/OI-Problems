## Description

<div><p>You are given an array $a_1,a_2,\ldots,a_n$ of length $n$ and a positive integer $k$, but some parts of the array $a$ are missing. Your task is to fill the missing part so that the <span class="tex-font-style-bf">maximum subarray sum</span>$^{\text{∗}}$ of $a$ is exactly $k$, or report that no solution exists.</p><p>Formally, you are given a binary string $s$ and a partially filled array $a$, where:</p><ul> <li> If you remember the value of $a_i$, $s_i = 1$ to indicate that, and you are given the real value of $a_i$. </li><li> If you don't remember the value of $a_i$, $s_i = 0$ to indicate that, and you are given $a_i = 0$. </li></ul><p>All the values that you remember satisfy $|a_i| \le 10^6$. However, you may use values up to $10^{18}$ to fill in the values that you do not remember. It can be proven that if a solution exists, a solution also exists satisfying $|a_i| \le 10^{18}$. </p><div class="statement-footnote"><p>$^{\text{∗}}$The <span class="tex-font-style-bf">maximum subarray sum</span> of an array $a$ of length $n$, i.e. $a_1, a_2, \ldots a_n$ is defined as $\max_{1 \le i \le j \le n} S(i, j)$ where $S(i, j) = a_i + a_{i + 1} + \ldots + a_j$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two numbers $n,k$ ($1 \le n \le 2 \cdot 10^5,1 \le k \le 10^{12}$).</p><p>The second line of each test case contains a binary ($\texttt{01}$) string $s$ of length $n$.</p><p>The third line of each test case contains $n$ numbers $a_1,a_2,\ldots,a_n$ ($|a_i| \le 10^6$). If $s_i = \texttt{0}$, then it's guaranteed that $a_i = 0$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>If there's at least one solution, print $n$ numbers $a_1,a_2,\ldots,a_n$ on the second line. $|a_i| \le 10^{18}$ must hold.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two numbers $n,k$ ($1 \le n \le 2 \cdot 10^5,1 \le k \le 10^{12}$).</p><p>The second line of each test case contains a binary ($\texttt{01}$) string $s$ of length $n$.</p><p>The third line of each test case contains $n$ numbers $a_1,a_2,\ldots,a_n$ ($|a_i| \le 10^6$). If $s_i = \texttt{0}$, then it's guaranteed that $a_i = 0$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>If there's at least one solution, print $n$ numbers $a_1,a_2,\ldots,a_n$ on the second line. $|a_i| \le 10^{18}$ must hold.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22,26,27,28
10
3 5
011
0 0 1
5 6
11011
4 -3 0 -2 1
4 4
0011
0 0 -4 -5
6 12
110111
1 2 0 5 -1 9
5 19
00000
0 0 0 0 0
5 19
11001
-8 6 0 0 -5
5 10
10101
10 0 10 0 10
1 1
1
0
3 5
111
3 -1 3
4 5
1011
-2 0 1 -5
```




```output1
Yes
4 0 1
Yes
4 -3 5 -2 1
Yes
2 2 -4 -5
No
Yes
5 1 9 2 2
Yes
-8 6 6 7 -5
Yes
10 -20 10 -20 10
No
Yes
3 -1 3
Yes
-2 4 1 -5
```



## Note

<p>In test case $1$, only the first position is not filled. We can fill it with $4$ to get the array $[4, 0, 1]$ which has maximum subarray sum of $5$.</p><p>In test case $2$, only the third position is not filled. We can fill it with $5$ to get the array $[4, -3, 5, -2, 1]$. Here the maximum subarray sum comes from the subarray $[4, -3, 5]$ and it is $6$, as required.</p><p>In test case $3$, the first and second positions are unfilled. We can fill both with $2$ to get the array $[2, 2, -4, -5]$ which has a maximum subarray sum of $4$. Note that other outputs are also possible such as $[0, 4, -4, -5]$.</p><p>In test case $4$, it is impossible to get a valid array. For example, if we filled the third position with $0$, we get $[1, 2, 0, 5, -1, 9]$, but this has a maximum subarray sum of $16$, not $12$ as required.</p>
