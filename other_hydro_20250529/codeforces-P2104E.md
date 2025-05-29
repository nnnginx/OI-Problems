## Description

<div><p>Let's call a letter <span class="tex-font-style-it">allowed</span> if it is a lowercase letter and is one of the first $k$ letters of the Latin alphabet.</p><p>You are given a string $s$ of length $n$, consisting only of allowed letters.</p><p>Let's call a string $t$ <span class="tex-font-style-it">pleasant</span> if $t$ is a subsequence of $s$.</p><p>You are given $q$ strings $t_1, t_2, \dots, t_q$. All of them consist only of allowed letters. For each string $t_i$, calculate the minimum number of allowed letters you need to append to it on the right so that it <span class="tex-font-style-bf">stops</span> being pleasant.</p><p>A sequence $t$ is a subsequence of a sequence $s$ if $t$ can be obtained from $s$ by the deletion of several (possibly, zero or all) element from arbitrary positions. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 10^6$; $1 \le k \le 26$)&nbsp;！ the length of the string $s$ and the number of allowed letters.</p><p>The second line contains the string $s$, consisting of $n$ lowercase Latin letters. Each character of the string is one of the first $k$ letters of the Latin alphabet.</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>The next $q$ lines contain queries: one query per line. The $i$-th line contains the string $t_i$, consisting only of allowed letters.</p><p>Additional constraint on input: the total length of all $t_i$ does not exceed $10^6$.</p></div><div class="output-specification"><p>For each query, output one integer&nbsp;！ the minimum number of allowed letters that need to be appended to the string on the right so that it stops being pleasant.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 10^6$; $1 \le k \le 26$)&nbsp;！ the length of the string $s$ and the number of allowed letters.</p><p>The second line contains the string $s$, consisting of $n$ lowercase Latin letters. Each character of the string is one of the first $k$ letters of the Latin alphabet.</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>The next $q$ lines contain queries: one query per line. The $i$-th line contains the string $t_i$, consisting only of allowed letters.</p><p>Additional constraint on input: the total length of all $t_i$ does not exceed $10^6$.</p>

## Output

<p>For each query, output one integer&nbsp;！ the minimum number of allowed letters that need to be appended to the string on the right so that it stops being pleasant.</p>





```input1|
7 3
abacaba
3
cc
bcb
b
```




```input2|
5 1
aaaaa
6
a
aa
aaa
aaaa
aaaaa
aaaaaa
```




```output1
0
1
2
```




```output2
5
4
3
2
1
0
```



## Note

<p>In the first example: </p><ol> <li> The string <span class="tex-font-style-tt">cc</span> is already unpleasant, so nothing needs to be appended to it; </li><li> <span class="tex-font-style-tt">bcb</span> is pleasant, so at least one letter needs to be appended to the right: <span class="tex-font-style-tt">bcba</span> will not work, but <span class="tex-font-style-tt">bcbb</span> and <span class="tex-font-style-tt">bcbc</span> are unpleasant. </li><li> To <span class="tex-font-style-tt">b</span>, at least two letters need to be appended, since <span class="tex-font-style-tt">ba</span>, <span class="tex-font-style-tt">bb</span>, and <span class="tex-font-style-tt">bc</span> are pleasant. For example, we can obtain an unpleasant string <span class="tex-font-style-tt">bbb</span>. </li></ol>
