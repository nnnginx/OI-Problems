## Description

<div><p>Given a string $s$ that consists only of the first three letters of the Latin alphabet, meaning each character of the string is either <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, or <span class="tex-font-style-tt">c</span>.</p><p>Also given are $q$ operations that need to be performed on the string. In each operation, two letters $x$ and $y$ from the set of the first three letters of the Latin alphabet are provided, and for each operation, one of the following two actions must be taken:</p><ul> <li> change any (one) occurrence of the letter $x$ in the string $s$ to the letter $y$ (if at least one occurrence of the letter $x$ exists); </li><li> do nothing. </li></ul><p>The goal is to perform all operations in the given order in such a way that the string $s$ becomes lexicographically minimal.</p><p>Recall that a string $a$ is lexicographically less than a string $b$ if and only if one of the following conditions holds:</p><ul> <li> $a$ is a prefix of $b$, but $a \neq b$; </li><li> at the first position where $a$ and $b$ differ, the string $a$ has a letter that comes earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there are two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^{5}$)&nbsp;！ the length of the string $s$ and the number of operations.</p><p>In the second line of each test case, the string $s$ is given&nbsp;！ a string of exactly $n$ characters, each of which is <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, or <span class="tex-font-style-tt">c</span>.</p><p>The next $q$ lines of each test case contain the description of the operations. Each line contains two characters $x$ and $y$, each of which is <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, or <span class="tex-font-style-tt">c</span>.</p><p>Additional constraints on the input:</p><ul> <li> the sum of $n$ across all test cases does not exceed $2 \cdot 10^{5}$; </li><li> the sum of $q$ across all test cases does not exceed $2 \cdot 10^{5}$. </li></ul></div><div class="output-specification"><p>For each test case, output the lexicographically minimal string that can be obtained from $s$ using the given operations.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{3}$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>In the first line of each test case, there are two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^{5}$)&nbsp;！ the length of the string $s$ and the number of operations.</p><p>In the second line of each test case, the string $s$ is given&nbsp;！ a string of exactly $n$ characters, each of which is <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, or <span class="tex-font-style-tt">c</span>.</p><p>The next $q$ lines of each test case contain the description of the operations. Each line contains two characters $x$ and $y$, each of which is <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, or <span class="tex-font-style-tt">c</span>.</p><p>Additional constraints on the input:</p><ul> <li> the sum of $n$ across all test cases does not exceed $2 \cdot 10^{5}$; </li><li> the sum of $q$ across all test cases does not exceed $2 \cdot 10^{5}$. </li></ul>

## Output

<p>For each test case, output the lexicographically minimal string that can be obtained from $s$ using the given operations.</p>





```input1|2,3,4,5,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39
3
2 2
cb
c b
b a
10 10
bbbbbbbbbb
b a
b c
c b
b a
c a
b c
b c
b a
a b
c a
30 20
abcaababcbbcabcbbcabcbabbbbabc
b c
b c
c a
b c
b c
b a
b c
b c
b a
b a
b a
b a
c a
b c
c a
b c
c a
c a
b c
c b
```




```output1
ab
aaaaabbbbb
aaaaaaaaaaaaaaabbbabcbabbbbabc
```



## Note

<p>In the first test case, both operations need to be applied to the first letter:</p><ol> <li> after the first operation, $s = $ "<span class="tex-font-style-tt">bb</span>" </li><li> after the second operation, $s = $ "<span class="tex-font-style-tt">ab</span>" </li></ol><p>In the second test case, the string could change as follows:</p><ol> <li> "<span class="tex-font-style-tt">bbbbabbbbb</span>" (changed the $5$-th letter) </li><li> "<span class="tex-font-style-tt">cbbbabbbbb</span>" (changed the $1$-st letter) </li><li> "<span class="tex-font-style-tt">cbbbabbbbb</span>" (did nothing) </li><li> "<span class="tex-font-style-tt">cbbaabbbbb</span>" (changed the $4$-th letter) </li><li> "<span class="tex-font-style-tt">abbaabbbbb</span>" (changed the $1$-st letter) </li><li> "<span class="tex-font-style-tt">abcaabbbbb</span>" (changed the $3$-rd letter) </li><li> "<span class="tex-font-style-tt">abcaabbbbb</span>" (did nothing) </li><li> "<span class="tex-font-style-tt">aacaabbbbb</span>" (changed the $2$-nd letter) </li><li> "<span class="tex-font-style-tt">aacaabbbbb</span>" (did nothing) </li><li> "<span class="tex-font-style-tt">aaaaabbbbb</span>" (changed the $3$-rd letter) </li></ol>
