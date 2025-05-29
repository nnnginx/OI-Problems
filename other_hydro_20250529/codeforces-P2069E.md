## Description

<div><p>You are given a string $s$ consisting of characters <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span>.</p><p>Your task is to split it into blocks of length $1$ and $2$ in such a way that </p><ul> <li> there are no more than $a$ strings equal to "<span class="tex-font-style-tt">A</span>"; </li><li> there are no more than $b$ strings equal to "<span class="tex-font-style-tt">B</span>"; </li><li> there are no more than $ab$ strings "<span class="tex-font-style-tt">AB</span>"; </li><li> there are no more than $ba$ strings "<span class="tex-font-style-tt">BA</span>"; </li></ul><p>Strings "<span class="tex-font-style-tt">AA</span>" and "<span class="tex-font-style-tt">BB</span>" are prohibited. Each character of the initial string $s$ should belong to exactly one block.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Next, $t$ independent cases follow.</p><p>The first line of each test case contains a single string $s$ ($1 \le |s| \le 5 \cdot 10^5$) consisting only of characters <span class="tex-font-style-tt">A</span> and/or <span class="tex-font-style-tt">B</span>.</p><p>The second line of each test case contains four integers $a$, $b$, $ab$, and $ba$ ($0 \le a, b, ab, ba \le 5 \cdot 10^5$)&nbsp;！ the maximum allowed number of strings "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">AB</span>", and "<span class="tex-font-style-tt">BA</span>" correspondingly.</p><p>It's guaranteed that the total length of $s$ doesn't exceed $5 \cdot 10^5$ over all test cases.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it's possible to split string $s$. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Next, $t$ independent cases follow.</p><p>The first line of each test case contains a single string $s$ ($1 \le |s| \le 5 \cdot 10^5$) consisting only of characters <span class="tex-font-style-tt">A</span> and/or <span class="tex-font-style-tt">B</span>.</p><p>The second line of each test case contains four integers $a$, $b$, $ab$, and $ba$ ($0 \le a, b, ab, ba \le 5 \cdot 10^5$)&nbsp;！ the maximum allowed number of strings "<span class="tex-font-style-tt">A</span>", "<span class="tex-font-style-tt">B</span>", "<span class="tex-font-style-tt">AB</span>", and "<span class="tex-font-style-tt">BA</span>" correspondingly.</p><p>It's guaranteed that the total length of $s$ doesn't exceed $5 \cdot 10^5$ over all test cases.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it's possible to split string $s$. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1|2,3,6,7,10,11,14,15
7
A
0 0 10 10
B
0 1 0 0
ABA
0 0 1 1
ABBABAAB
5 5 0 0
ABABBAABBAAB
1 1 2 3
ABBBBAB
0 3 2 0
BAABBA
1 3 2 0
```




```output1
NO
YES
NO
YES
YES
YES
NO
```



## Note

<p>In the third test case, all possible splits are: <span class="tex-font-style-tt">A|B|A</span>, <span class="tex-font-style-tt">AB|A</span> or <span class="tex-font-style-tt">A|BA</span>. All of them have at least one "<span class="tex-font-style-tt">A</span>".</p><p>In the fourth test case, one of the possible splits is the following: <span class="tex-font-style-tt">A|B|B|A|B|A|A|B</span>.</p><p>In the fifth test case, one of the possible splits is the following: <span class="tex-font-style-tt">A|BA|B|BA|AB|BA|AB</span>.</p>
