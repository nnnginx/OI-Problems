## Description

<div><p>You are given two strings $a$ and $b$, both consisting of lowercase Latin letters. </p><p>A <span class="tex-font-style-it">subsequence</span> of a string is a string which can be obtained by removing several (possibly zero) characters from the original string. A <span class="tex-font-style-it">substring</span> of a string is a contiguous subsequence of that string.</p><p>For example, consider the string <span class="tex-font-style-tt">abac</span>:</p><ul> <li> <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">aa</span>, <span class="tex-font-style-tt">ac</span>, <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">bc</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">abc</span>, <span class="tex-font-style-tt">aac</span>, <span class="tex-font-style-tt">bac</span> and <span class="tex-font-style-tt">abac</span> are its subsequences; </li><li> <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">ab</span>, <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">ac</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">bac</span> and <span class="tex-font-style-tt">abac</span> are its substrings. </li></ul><p>Your task is to calculate the minimum possible length of the string that contains $a$ as a substring and $b$ as a subsequence.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a string $a$ ($1 \le |a| \le 100$), consisting of lowercase Latin letters.</p><p>The second line of each test case contains a string $b$ ($1 \le |b| \le 100$), consisting of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum possible length of the string that contains $a$ as a substring and $b$ as a subsequence.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^3$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a string $a$ ($1 \le |a| \le 100$), consisting of lowercase Latin letters.</p><p>The second line of each test case contains a string $b$ ($1 \le |b| \le 100$), consisting of lowercase Latin letters.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum possible length of the string that contains $a$ as a substring and $b$ as a subsequence.</p>





```input1|2,3,6,7,10,11
5
aba
cb
er
cf
mmm
mmm
contest
test
cde
abcefg
```




```output1
4
4
3
7
7
```



## Note

<p>In the examples below, the characters that correspond to the subsequence equal to $b$ are bolded.</p><p>In the first example, one of the possible answers is <span class="tex-font-style-tt"><span class="tex-font-style-bf">c</span>a<span class="tex-font-style-bf">b</span>a</span>.</p><p>In the second example, one of the possible answers is <span class="tex-font-style-tt">er<span class="tex-font-style-bf">cf</span></span>.</p><p>In the third example, one of the possible answers is <span class="tex-font-style-tt"><span class="tex-font-style-bf">mmm</span></span>.</p><p>In the fourth example, one of the possible answers is <span class="tex-font-style-tt">con<span class="tex-font-style-bf">test</span></span>.</p><p>In the fifth example, one of the possible answers is <span class="tex-font-style-tt"><span class="tex-font-style-bf">abc</span>d<span class="tex-font-style-bf">efg</span></span>.</p>
