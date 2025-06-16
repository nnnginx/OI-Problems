## Description

<div><p>Let's define a <span class="tex-font-style-it">cyclic shift</span> of some string $s$ as a transformation from $s_1 s_2 \dots s_{n-1} s_{n}$ into $s_{n} s_1 s_2 \dots s_{n-1}$. In other words, you take one last character $s_n$ and place it before the first character while moving all other characters to the right.</p><p>You are given a binary string $s$ (a string consisting of only <span class="tex-font-style-tt">0</span>-s and/or <span class="tex-font-style-tt">1</span>-s).</p><p>In one operation, you can choose any substring $s_l s_{l+1} \dots s_r$ ($1 \le l &lt; r \le |s|$) and cyclically shift it. The <span class="tex-font-style-it">cost</span> of such operation is equal to $r - l + 1$ (or the length of the chosen substring).</p><p>You can perform the given operation any number of times. What is the minimum <span class="tex-font-style-bf">total</span> cost to make $s$ sorted in non-descending order?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains a binary string $s$ ($2 \le |s| \le 2 \cdot 10^5$; $s_i \in$ {<span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>})&nbsp;！ the string you need to sort.</p><p>Additional constraint on the input: the sum of lengths of strings over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the single integer&nbsp;！ the minimum total cost to make string sorted using operation above any number of times.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first and only line of each test case contains a binary string $s$ ($2 \le |s| \le 2 \cdot 10^5$; $s_i \in$ {<span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>})&nbsp;！ the string you need to sort.</p><p>Additional constraint on the input: the sum of lengths of strings over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the single integer&nbsp;！ the minimum total cost to make string sorted using operation above any number of times.</p>





```input1|2,4,6
5
10
0000
11000
101011
01101001
```




```output1
2
0
9
5
11
```



## Note

<p>In the first test case, you can choose the whole string and perform a cyclic shift: <span class="tex-font-style-tt">10</span> $\rightarrow$ <span class="tex-font-style-tt">01</span>. The length of the substring is $2$, so the cost is $2$.</p><p>In the second test case, the string is already sorted, so you don't need to perform any operations.</p><p>In the third test case, one of the optimal strategies is the next: </p><ol> <li> choose substring $[1, 3]$: <span class="tex-font-style-tt">11000</span> $\rightarrow$ <span class="tex-font-style-tt">01100</span>; </li><li> choose substring $[2, 4]$: <span class="tex-font-style-tt">01100</span> $\rightarrow$ <span class="tex-font-style-tt">00110</span>; </li><li> choose substring $[3, 5]$: <span class="tex-font-style-tt">00110</span> $\rightarrow$ <span class="tex-font-style-tt">00011</span>. </li></ol> The total cost is $3 + 3 + 3 = 9$.
