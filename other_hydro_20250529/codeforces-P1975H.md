## Description

<div><p>378QAQ has a string $s$ of length $n$. Define the <span class="tex-font-style-it">core</span> of a string as the substring$^\dagger$ with maximum lexicographic$^\ddagger$ order.</p><p>For example, the core of "$\mathtt{bazoka}$" is "$\mathtt{zoka}$", and the core of "$\mathtt{aaa}$" is "$\mathtt{aaa}$".</p><p>378QAQ wants to rearrange the string $s$ so that the core is lexicographically minimum. Find the lexicographically minimum possible core over all rearrangements of $s$.</p><p>$^\dagger$ A substring of string $s$ is a continuous segment of letters from $s$. For example, "$\mathtt{defor}$", "$\mathtt{code}$" and "$\mathtt{o}$" are all substrings of "$\mathtt{codeforces}$" while "$\mathtt{codes}$" and "$\mathtt{aaa}$" are not.</p><p>$^\ddagger$ A string $p$ is lexicographically smaller than a string $q$ if and only if one of the following holds: </p><ul> <li> $p$ is a prefix of $q$, but $p \ne q$; or </li><li> in the first position where $p$ and $q$ differ, the string $p$ has a smaller element than the corresponding element in $q$ (when compared by their ASCII code). </li></ul><p>For example, "$\mathtt{code}$" and "$\mathtt{coda}$" are both lexicographically smaller than "$\mathtt{codeforces}$" while "$\mathtt{codeforceston}$" and "$\mathtt{z}$" are not.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 10^6$)&nbsp;¡ª the length of string $s$.</p><p>The next line of each test case contains the string $s$ of length $n$. The string $s$ consists of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output the lexicographically minimum possible core over all rearrangements of $s$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 10^6$)&nbsp;¡ª the length of string $s$.</p><p>The next line of each test case contains the string $s$ of length $n$. The string $s$ consists of lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output the lexicographically minimum possible core over all rearrangements of $s$.</p>





```input1|2,3,6,7,10,11
6
3
qaq
4
cccc
6
bazoka
6
zazzzz
7
ababbbb
7
ccbabcc
```




```output1
qaq
cccc
z
zzz
bbababb
cbcacbc
```



## Note

<p>In the first test case, all possible rearrangements and their corresponding cores are as follows: </p><ul> <li> "$\mathtt{qaq}$", its core is "$\mathtt{qaq}$". </li><li> "$\mathtt{aqq}$", its core is "$\mathtt{qq}$". </li><li> "$\mathtt{qqa}$", its core is "$\mathtt{qqa}$". </li></ul><p>So the core with the minimum lexicographic order in all rearrangement plans is "$\mathtt{qaq}$".</p>
