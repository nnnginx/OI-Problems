## Description

<div><p>Vasya has a string $s$ of length $n$. He decides to make the following modification to the string: </p><ol> <li> Pick an integer $k$, ($1 \leq k \leq n$). </li><li> For $i$ from $1$ to $n-k+1$, reverse the substring $s[i:i+k-1]$ of $s$. For example, if string $s$ is <span class="tex-font-style-tt">qwer</span> and $k = 2$, below is the series of transformations the string goes through: <ul> <li> <span class="tex-font-style-tt">qwer</span> (original string) </li><li> <span class="tex-font-style-tt">wqer</span> (after reversing the first substring of length $2$) </li><li> <span class="tex-font-style-tt">weqr</span> (after reversing the second substring of length $2$) </li><li> <span class="tex-font-style-tt">werq</span> (after reversing the last substring of length $2$) </li></ul> Hence, the resulting string after modifying $s$ with $k = 2$ is <span class="tex-font-style-tt">werq</span>. </li></ol><p>Vasya wants to choose a $k$ such that the string obtained after the above-mentioned modification is lexicographically smallest possible among all choices of $k$. Among all such $k$, he wants to choose the smallest one. Since he is busy attending Felicity 2020, he asks for your help.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;�� the length of the string $s$.</p><p>The second line of each test case contains the string $s$ of $n$ lowercase latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each testcase output two lines:</p><p>In the first line output the lexicographically smallest string $s'$ achievable after the above-mentioned modification. </p><p>In the second line output the appropriate value of $k$ ($1 \leq k \leq n$) that you chose for performing the modification. If there are multiple values of $k$ that give the lexicographically smallest string, output the smallest value of $k$ among them.</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;�� the length of the string $s$.</p><p>The second line of each test case contains the string $s$ of $n$ lowercase latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each testcase output two lines:</p><p>In the first line output the lexicographically smallest string $s'$ achievable after the above-mentioned modification. </p><p>In the second line output the appropriate value of $k$ ($1 \leq k \leq n$) that you chose for performing the modification. If there are multiple values of $k$ that give the lexicographically smallest string, output the smallest value of $k$ among them.</p>

## Samples

```input1
6
4
abab
6
qwerty
5
aaaaa
6
alaska
9
lfpbavjsm
1
p
```

```output1
abab
1
ertyqw
3
aaaaa
1
aksala
6
avjsmbpfl
5
p
1
```




## Note

<p>In the first testcase of the first sample, the string modification results for the sample <span class="tex-font-style-tt">abab</span> are as follows : </p><ul> <li> for $k = 1$ : <span class="tex-font-style-tt">abab</span> </li><li> for $k = 2$ : <span class="tex-font-style-tt">baba</span> </li><li> for $k = 3$ : <span class="tex-font-style-tt">abab</span> </li><li> for $k = 4$ : <span class="tex-font-style-tt">baba</span><p>The lexicographically smallest string achievable through modification is <span class="tex-font-style-tt">abab</span> for $k = 1$ and $3$. Smallest value of $k$ needed to achieve is hence $1$. </p></li></ul>
