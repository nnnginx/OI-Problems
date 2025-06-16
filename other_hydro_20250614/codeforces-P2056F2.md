## Description

<div><p>  </p><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that in this version, the constraints on $t$, $k$, and $m$ are higher. You can hack only if you solved all versions of this problem.</span> </p><p>A sequence $a$ of $n$ integers is called <span class="tex-font-style-it">good</span> if the following condition holds:</p><ul> <li> Let $\text{cnt}_x$ be the number of occurrences of $x$ in sequence $a$. For all pairs $0 \le i &lt; j &lt; m$, at least one of the following has to be true: $\text{cnt}_i = 0$, $\text{cnt}_j = 0$, or $\text{cnt}_i \le \text{cnt}_j$. In other words, if both $i$ and $j$ are present in sequence $a$, then the number of occurrences of $i$ in $a$ is less than or equal to the number of occurrences of $j$ in $a$. </li></ul><p>You are given integers $n$ and $m$. Calculate the value of the bitwise XOR of the median$^{\text{∗}}$ of all good sequences $a$ of length $n$ with $0\le a_i &lt; m$. </p><p>Note that the value of $n$ can be very large, so you are given its binary representation instead.</p><div class="statement-footnote"><p>$^{\text{∗}}$The median of a sequence $a$ of length $n$ is defined as the $\left\lfloor\frac{n + 1}{2}\right\rfloor$-th smallest value in the sequence.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $k$ and $m$ ($1 \le k \le 2 \cdot 10^5$, $1 \le m \le 10^9$)&nbsp;— the number of bits in $n$ and the upper bound on the elements in sequence $a$.</p><p>The second line of each test case contains a binary string of length $k$&nbsp;— the binary representation of $n$ with no leading zeros.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $2\cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer representing the bitwise XOR of the median of all good sequences $a$ of length $n$ where $0\le a_i &lt; m$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $k$ and $m$ ($1 \le k \le 2 \cdot 10^5$, $1 \le m \le 10^9$)&nbsp;— the number of bits in $n$ and the upper bound on the elements in sequence $a$.</p><p>The second line of each test case contains a binary string of length $k$&nbsp;— the binary representation of $n$ with no leading zeros.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $2\cdot 10^5$. </p>

## Output

<p>For each test case, output a single integer representing the bitwise XOR of the median of all good sequences $a$ of length $n$ where $0\le a_i &lt; m$.</p>





```input1|2,3,6,7,10,11
6
2 3
10
2 3
11
5 1
11101
7 9
1101011
17 34
11001010001010010
1 1000000000
1
```




```output1
3
2
0
8
32
0
```



## Note

<p>In the first example, $n = 10_2 = 2$ and $m = 3$. All possible sequences with elements less than $m$ are: $[0, 0]$, $[0, 1]$, $[0, 2]$, $[1, 0]$, $[1, 1]$, $[1, 2]$, $[2, 0]$, $[2, 1]$, $[2, 2]$. All of them are good, so the answer is: $0 \oplus 0 \oplus 0 \oplus 0 \oplus 1 \oplus 1 \oplus 0 \oplus 1 \oplus 2 = 3$.</p><p>In the second example, $n = 11_2 = 3$ and $m = 3$. Some good sequences are $[2, 2, 2]$, $[1, 0, 1]$, and $[2, 0, 1]$. However, a sequence $[2, 0, 0]$ is not good, because $\text{cnt}_0 = 2$, $\text{cnt}_2 = 1$. Therefore, if we set $i = 0$ and $j = 2$, $i &lt; j$ holds, but $\text{cnt}_i \le \text{cnt}_j$ does not.</p>
