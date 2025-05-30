## Description

<div><p>A bitstring is a string consisting only of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. A bitstring is called $k$-<span class="tex-font-style-bf">balanced</span> if every substring of size $k$ of this bitstring has an equal amount of <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> characters ($\frac{k}{2}$ of each).</p><p>You are given an integer $k$ and a string $s$ which is composed only of characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>. You need to determine whether you can make a $k$-balanced bitstring by replacing every <span class="tex-font-style-tt">?</span> characters in $s$ with either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 3 \cdot 10^5$, $k$ is even) &nbsp;�� the length of the string and the parameter for a balanced bitstring.</p><p>The next line contains the string $s$ ($|s| = n$). It is given that $s$ consists of only <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if we can replace every <span class="tex-font-style-tt">?</span> in $s$ with <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> such that the resulting bitstring is $k$-balanced, or <span class="tex-font-style-tt">NO</span> if it is not possible.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le k \le n \le 3 \cdot 10^5$, $k$ is even) &nbsp;�� the length of the string and the parameter for a balanced bitstring.</p><p>The next line contains the string $s$ ($|s| = n$). It is given that $s$ consists of only <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if we can replace every <span class="tex-font-style-tt">?</span> in $s$ with <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> such that the resulting bitstring is $k$-balanced, or <span class="tex-font-style-tt">NO</span> if it is not possible.</p>

## Samples

```input1
9
6 4
100110
3 2
1?1
3 2
1?0
4 4
????
7 4
1?0??1?
10 10
11??11??11
4 2
1??1
4 4
?0?0
6 2
????00
```

```output1
YES
YES
NO
YES
YES
NO
NO
YES
NO
```




## Note

<p>For the first test case, the string is already a $4$-balanced bitstring.</p><p>For the second test case, the string can be transformed into <span class="tex-font-style-tt">101</span>.</p><p>For the fourth test case, the string can be transformed into <span class="tex-font-style-tt">0110</span>.</p><p>For the fifth test case, the string can be transformed into <span class="tex-font-style-tt">1100110</span>.</p>
