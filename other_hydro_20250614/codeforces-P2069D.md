## Description

<div><p>You are given a string $s$ consisting of lowercase Latin letters.</p><p>You can perform the following operation with the string $s$: choose a contiguous substring (possibly empty) of $s$ and shuffle it (reorder the characters in the substring as you wish).</p><p>Recall that a palindrome is a string that reads the same way from the first character to the last and from the last character to the first. For example, the strings <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">bab</span>, <span class="tex-font-style-tt">acca</span>, <span class="tex-font-style-tt">bcabcbacb</span> are palindromes, but the strings <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">abbbaa</span>, <span class="tex-font-style-tt">cccb</span> are not.</p><p>Your task is to determine the minimum possible length of the substring on which the aforementioned operation must be performed in order to convert the given string $s$ into a palindrome.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ ($2 \le |s| \le 2 \cdot 10^5$), consisting of lowercase Latin letters.</p><p>Additional constraints on the input: </p><ul> <li> the string $s$ has an even length; </li><li> the string $s$ can always be converted to a palindrome; </li><li> the sum of lengths of $s$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum possible length of the substring on which the aforementioned operation must be performed in order to convert the given string $s$ into a palindrome.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a string $s$ ($2 \le |s| \le 2 \cdot 10^5$), consisting of lowercase Latin letters.</p><p>Additional constraints on the input: </p><ul> <li> the string $s$ has an even length; </li><li> the string $s$ can always be converted to a palindrome; </li><li> the sum of lengths of $s$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum possible length of the substring on which the aforementioned operation must be performed in order to convert the given string $s$ into a palindrome.</p>





```input1|2,4
4
baba
cc
ddaa
acbacddacbca
```




```output1
2
0
3
2
```



## Note

<p>In the first example, you can perform the operation as follows: <span class="tex-font-style-tt">ba<span class="tex-font-style-underline">ba</span></span> $\rightarrow$ <span class="tex-font-style-tt">ba<span class="tex-font-style-underline">ab</span></span>.</p><p>In the second example, the string is already a palindrome, so we can shuffle an empty substring.</p><p>In the third example, you can perform the operation as follows: <span class="tex-font-style-tt"><span class="tex-font-style-underline">dda</span>a</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-underline">add</span>a</span>.</p><p>In the fourth example, you can perform the operation as follows: <span class="tex-font-style-tt">acb<span class="tex-font-style-underline">ac</span>ddacbca</span> $\rightarrow$ <span class="tex-font-style-tt">acb<span class="tex-font-style-underline">ca</span>ddacbca</span>.</p>
