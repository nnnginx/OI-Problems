## Description

<div><p>For an array $b$ of length $m$, define $f(b)$ as follows.</p><p>Consider a $1 \times m$ strip, where all cells initially have darkness $0$. You want to transform it into a strip where the color at the $i$-th position has darkness $b_i$. You can perform the following operation, which consists of two steps:</p><ol><li> Fold the paper at any line between two cells. You may fold as many times as you like, or choose not to fold at all.</li><li> Choose <span class="tex-font-style-bf">one</span> position to drop the black dye. The dye permeates from the top and flows down to the bottom, increasing the darkness of all cells in its path by $1$. After dropping the dye, you unfold the strip.</li></ol><p>Let $f(b)$ be the minimum number of operations required to achieve the desired configuration. It can be proven that the goal can always be achieved in a finite number of operations.</p><p>You are given an array $a$ of length $n$. Evaluate</p><p>$$\sum_{l=1}^n\sum_{r=l}^n f(a_l a_{l+1} \ldots a_r)$$</p><p>modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;！ denoting the array $a$.</p><p>It is guaranteed that the sum of all values of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the required sum modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;！ denoting the array $a$.</p><p>It is guaranteed that the sum of all values of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the required sum modulo $998\,244\,353$.</p>





```input1|2,3,6,7
4
3
0 1 0
6
1 0 0 1 2 1
5
2 1 2 4 3
12
76 55 12 32 11 45 9 63 88 83 32 6
```




```output1
4
28
47
7001
```



## Note

<p>In the first test case, </p><ul> <li> $f(a_1)=f(\mathtt{0})=0$ </li><li> $f(a_1a_2)=f(\mathtt{01})=1$ </li><li> $f(a_1a_2a_3)=f(\mathtt{010})=1$ </li><li> $f(a_2)=f(\mathtt{1})=1$ </li><li> $f(a_2a_3)=f(\mathtt{10})=1$ </li><li> $f(a_3)=f(\mathtt{0})=0$ </li></ul><p>This sums up to $0+1+1+1+1+0 = 4$</p><p>In the second test case, $f(a_1a_2a_3a_4a_5a_6) = 2$. Here's one possible sequence of operations.</p><center> <img class="tex-graphics" src="./36007/file/2vjJTjT3.png" style="max-width: 100.0%;max-height: 100.0%;">   </center>
