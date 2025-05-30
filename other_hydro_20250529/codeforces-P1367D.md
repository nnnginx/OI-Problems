## Description

<div><p>Polycarp wrote on the board a string $s$ containing only lowercase Latin letters ('<span class="tex-font-style-tt">a</span>'-'<span class="tex-font-style-tt">z</span>'). This string is known for you and given in the input.</p><p>After that, he erased some letters from the string $s$, and he rewrote the remaining letters in <span class="tex-font-style-bf">any</span> order. As a result, he got some new string $t$. You have to find it with some additional information.</p><p>Suppose that the string $t$ has length $m$ and the characters are numbered from left to right from $1$ to $m$. You are given a sequence of $m$ integers: $b_1, b_2, \ldots, b_m$, where $b_i$ is the sum of the distances $|i-j|$ from the index $i$ to all such indices $j$ that $t_j &gt; t_i$ (consider that '<span class="tex-font-style-tt">a</span>'&lt;'<span class="tex-font-style-tt">b</span>'&lt;...&lt;'<span class="tex-font-style-tt">z</span>'). In other words, to calculate $b_i$, Polycarp finds all such indices $j$ that the index $j$ contains a letter that is later in the alphabet than $t_i$ and sums all the values $|i-j|$.</p><p>For example, if $t$ = "<span class="tex-font-style-tt">abzb</span>", then:</p><ul> <li> since $t_1$='<span class="tex-font-style-tt">a</span>', all other indices contain letters which are later in the alphabet, that is: $b_1=|1-2|+|1-3|+|1-4|=1+2+3=6$; </li><li> since $t_2$='<span class="tex-font-style-tt">b</span>', only the index $j=3$ contains the letter, which is later in the alphabet, that is: $b_2=|2-3|=1$; </li><li> since $t_3$='<span class="tex-font-style-tt">z</span>', then there are no indexes $j$ such that $t_j&gt;t_i$, thus $b_3=0$; </li><li> since $t_4$='<span class="tex-font-style-tt">b</span>', only the index $j=3$ contains the letter, which is later in the alphabet, that is: $b_4=|4-3|=1$. </li></ul><p>Thus, if $t$ = "<span class="tex-font-style-tt">abzb</span>", then $b=[6,1,0,1]$.</p><p>Given the string $s$ and the array $b$, find any possible string $t$ for which the following two requirements are fulfilled simultaneously:</p><ul> <li> $t$ is obtained from $s$ by erasing some letters (possibly zero) and then writing the rest in <span class="tex-font-style-bf">any</span> order; </li><li> the array, constructed from the string $t$ according to the rules above, equals to the array $b$ specified in the input data. </li></ul></div><div class="input-specification"><p>The first line contains an integer $q$ ($1 \le q \le 100$)&nbsp;�� the number of test cases in the test. Then $q$ test cases follow.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains string $s$, which has a length from $1$ to $50$ and consists of lowercase English letters; </li><li> the second line contains positive integer $m$ ($1 \le m \le |s|$), where $|s|$ is the length of the string $s$, and $m$ is the length of the array $b$; </li><li> the third line contains the integers $b_1, b_2, \dots, b_m$ ($0 \le b_i \le 1225$). </li></ul><p>It is guaranteed that in each test case an answer exists.</p></div><div class="output-specification"><p>Output $q$ lines: the $k$-th of them should contain the answer (string $t$) to the $k$-th test case. It is guaranteed that an answer to each test case exists. If there are several answers, output any.</p></div>

## Input

<p>The first line contains an integer $q$ ($1 \le q \le 100$)&nbsp;�� the number of test cases in the test. Then $q$ test cases follow.</p><p>Each test case consists of three lines:</p><ul> <li> the first line contains string $s$, which has a length from $1$ to $50$ and consists of lowercase English letters; </li><li> the second line contains positive integer $m$ ($1 \le m \le |s|$), where $|s|$ is the length of the string $s$, and $m$ is the length of the array $b$; </li><li> the third line contains the integers $b_1, b_2, \dots, b_m$ ($0 \le b_i \le 1225$). </li></ul><p>It is guaranteed that in each test case an answer exists.</p>

## Output

<p>Output $q$ lines: the $k$-th of them should contain the answer (string $t$) to the $k$-th test case. It is guaranteed that an answer to each test case exists. If there are several answers, output any.</p>

## Samples

```input1
4
abac
3
2 1 0
abc
1
0
abba
3
1 0 1
ecoosdcefr
10
38 13 24 14 11 5 3 24 17 0
```

```output1
aac
b
aba
codeforces
```




## Note

<p>In the first test case, such strings $t$ are suitable: "<span class="tex-font-style-tt">aac</span>', "<span class="tex-font-style-tt">aab</span>".</p><p>In the second test case, such trings $t$ are suitable: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>".</p><p>In the third test case, only the string $t$ equals to "<span class="tex-font-style-tt">aba</span>" is suitable, but the character '<span class="tex-font-style-tt">b</span>' can be from the second or third position.</p>
