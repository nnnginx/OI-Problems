## Description

<div><p>Vlad found a binary string$^{\text{∗}}$ $s$ of even length $n$. He considers a pair of indices ($i, n - i + 1$), where $1 \le i &lt; n - i + 1$, to be good if $s_i = s_{n - i + 1}$ holds true.</p><p>For example, in the string '<span class="tex-font-style-tt">010001</span>' there is only $1$ good pair, since $s_1 \ne s_6$, $s_2 \ne s_5$, and $s_3=s_4$. In the string '<span class="tex-font-style-tt">0101</span>' there are no good pairs.</p><p>Vlad loves palindromes, but not too much, so he wants to rearrange some characters of the string so that there are exactly $k$ good pairs of indices.</p><p>Determine whether it is possible to rearrange the characters in the given string so that there are exactly $k$ good pairs of indices ($i, n - i + 1$).</p><div class="statement-footnote"><p>$^{\text{∗}}$A string $s$ is called binary if it consists only of the characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' </p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $0 \le k \le \frac{n}{2}$, $n$ is even)&nbsp;— the length of the string and the required number of good pairs.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if there is a way to rearrange the characters of the string so that there are exactly $k$ good pairs, otherwise output "<span class="tex-font-style-tt">NO</span>".</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $0 \le k \le \frac{n}{2}$, $n$ is even)&nbsp;— the length of the string and the required number of good pairs.</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if there is a way to rearrange the characters of the string so that there are exactly $k$ good pairs, otherwise output "<span class="tex-font-style-tt">NO</span>".</p><p>You may output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,3,6,7,10,11
6
6 2
000000
2 1
01
4 1
1011
10 2
1101011001
10 1
1101011001
2 1
11
```




```output1
NO
NO
YES
NO
YES
YES
```


