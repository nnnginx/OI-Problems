## Description

<div><p> </p><p>You have an array $a$ of size $n$ — $a_1, a_2, \ldots a_n$. </p><p>You need to divide the $n$ elements into $2$ sequences $B$ and $C$, satisfying the following conditions:</p><ul> <li> Each element belongs to exactly one sequence. </li><li> Both sequences $B$ and $C$ contain at least one element. </li><li> $\gcd$ $(B_1, B_2, \ldots, B_{|B|}) \ne \gcd(C_1, C_2, \ldots, C_{|C|})$ $^{\text{∗}}$ </li></ul><div class="statement-footnote"><p>$^{\text{∗}}$$\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 100$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^4$).</p></div><div class="output-specification"><p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>Only when there is a solution, output $n$ integers on the second line. The $i$-th number should be either $1$ or $2$. $1$ represents that the element belongs to sequence $B$ and $2$ represents that the element belongs to sequence $C$. </p><p>You should guarantee that $1$ and $2$ both appear at least once.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 100$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 10^4$).</p>

## Output

<p>For each test case, first output $\texttt{Yes}$ if a solution exists or $\texttt{No}$ if no solution exists. You may print each character in either case, for example $\texttt{YES}$ and $\texttt{yEs}$ will also be accepted.</p><p>Only when there is a solution, output $n$ integers on the second line. The $i$-th number should be either $1$ or $2$. $1$ represents that the element belongs to sequence $B$ and $2$ represents that the element belongs to sequence $C$. </p><p>You should guarantee that $1$ and $2$ both appear at least once.</p>





```input1|2,3,6,7
3
4
1 20 51 9
4
5 5 5 5
3
1 2 2
```




```output1
Yes
2 2 1 1
No
Yes
1 2 2
```



## Note

<p>In the first test case, $B = [51, 9]$ and $C = [1, 20]$. You can verify $\gcd(B_1, B_2) = 3 \ne 1 = \gcd(C_1, C_2)$.</p><p>In the second test case, it is impossible to find a solution. For example, suppose you distributed the first $3$ elements to array $B$ and then the last element to array $C$. You have $B = [5, 5, 5]$ and $C = [5]$, but $\gcd(B_1, B_2, B_3) = 5 = \gcd(C_1)$. Hence it is invalid.</p>
