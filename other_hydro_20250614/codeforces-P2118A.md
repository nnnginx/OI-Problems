## Description

<div><p>We call a bitstring$^{\text{∗}}$ perfect if it has the same number of $\mathtt{101}$ and $\mathtt{010}$ subsequences$^{\text{†}}$. Construct a perfect bitstring of length $n$ where the number of $\mathtt{1}$ characters it contains is exactly $k$.</p><p>It can be proven that the construction is always possible. If there are multiple solutions, output any of them.</p><div class="statement-footnote"><p>$^{\text{∗}}$A bitstring is a string consisting only of the characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>$^{\text{†}}$A sequence $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by the deletion of several (possibly zero or all) characters.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le n$)&nbsp;— the size of the bitstring and the number of $\mathtt{1}$ characters in the bitstring.</p></div><div class="output-specification"><p>For each test case, output the constructed bitstring. If there are multiple solutions, output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 100$, $0 \le k \le n$)&nbsp;— the size of the bitstring and the number of $\mathtt{1}$ characters in the bitstring.</p>

## Output

<p>For each test case, output the constructed bitstring. If there are multiple solutions, output any of them.</p>





```input1|2,4,6
5
4 2
5 3
5 5
6 2
1 1
```




```output1
1010
10110
11111
100010
1
```



## Note

<p>In the first test case, the number of $\mathtt{101}$ and $\mathtt{010}$ subsequences is the same, both being $1$, and the sequence contains exactly two $\mathtt{1}$ characters.</p><p>In the second test case, the number of $\mathtt{101}$ and $\mathtt{010}$ subsequences is the same, both being $2$, and the sequence contains exactly three $\mathtt{1}$ characters.</p><p>In the third test case, the number of $\mathtt{101}$ and $\mathtt{010}$ subsequences is the same, both being $0$, and the sequence contains exactly five $\mathtt{1}$ characters.</p>
