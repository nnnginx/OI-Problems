## Description

<div><p>You are given a binary string $s$ of length $n$, consisting of zeros and ones. You can perform the following operation <span class="tex-font-style-bf">exactly once</span>:</p><ol> <li> Choose an integer $p$ ($1 \le p \le n$). </li><li> Reverse the substring $s_1 s_2 \ldots s_p$. After this step, the string $s_1 s_2 \ldots s_n$ will become $s_p s_{p-1} \ldots s_1 s_{p+1} s_{p+2} \ldots s_n$. </li><li> Then, perform a cyclic shift of the string $s$ to the left $p$ times. After this step, the initial string $s_1s_2 \ldots s_n$ will become $s_{p+1}s_{p+2} \ldots s_n s_p s_{p-1} \ldots s_1$. </li></ol><p>For example, if you apply the operation to the string <span class="tex-font-style-tt">110001100110</span> with $p=3$, after the second step, the string will become <span class="tex-font-style-tt"><span class="tex-font-style-bf">011</span>001100110</span>, and after the third step, it will become <span class="tex-font-style-tt">001100110<span class="tex-font-style-bf">011</span></span>.</p><p>A string $s$ is called <span class="tex-font-style-it">$k$-proper</span> if two conditions are met:</p><ul> <li> $s_1=s_2=\ldots=s_k$; </li><li> $s_{i+k} \neq s_i$ for any $i$ ($1 \le i \le n - k$). </li></ul><p>For example, with $k=3$, the strings <span class="tex-font-style-tt">000</span>, <span class="tex-font-style-tt">111000111</span>, and <span class="tex-font-style-tt">111000</span> are $k$-proper, while the strings <span class="tex-font-style-tt">000000</span>, <span class="tex-font-style-tt">001100</span>, and <span class="tex-font-style-tt">1110000</span> are not.</p><p>You are given an integer $k$, which <span class="tex-font-style-bf">is a divisor</span> of $n$. Find an integer $p$ ($1 \le p \le n$) such that after performing the operation, the string $s$ becomes $k$-proper, or determine that it is impossible. Note that if the string is initially $k$-proper, you still need to apply exactly one operation to it.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n$, $2 \le n \le 10^5$)&nbsp;！ the length of the string $s$ and the value of $k$. It is guaranteed that $k$ <span class="tex-font-style-bf">is a divisor</span> of $n$.</p><p>The second line of each test case contains a binary string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the value of $p$ to make the string $k$-proper, or $-1$ if it is impossible.</p><p>If there are multiple solutions, output any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n$, $2 \le n \le 10^5$)&nbsp;！ the length of the string $s$ and the value of $k$. It is guaranteed that $k$ <span class="tex-font-style-bf">is a divisor</span> of $n$.</p><p>The second line of each test case contains a binary string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the value of $p$ to make the string $k$-proper, or $-1$ if it is impossible.</p><p>If there are multiple solutions, output any of them.</p>





```input1|2,3,6,7,10,11,14,15
7
8 4
11100001
4 2
1110
12 3
111000100011
5 5
00000
6 1
101001
8 4
01110001
12 2
110001100110
```




```output1
3
-1
7
5
4
-1
3
```



## Note

<p>In the first test case, if you apply the operation with $p=3$, after the second step of the operation, the string becomes <span class="tex-font-style-tt"><span class="tex-font-style-bf">111</span>00001</span>, and after the third step, it becomes <span class="tex-font-style-tt">00001<span class="tex-font-style-bf">111</span></span>. This string is $4$-proper.</p><p>In the second test case, it can be shown that there is no operation after which the string becomes $2$-proper.</p><p>In the third test case, if you apply the operation with $p=7$, after the second step of the operation, the string becomes <span class="tex-font-style-tt"><span class="tex-font-style-bf">1000111</span>00011</span>, and after the third step, it becomes <span class="tex-font-style-tt">00011<span class="tex-font-style-bf">1000111</span></span>. This string is $3$-proper.</p><p>In the fourth test case, after the operation with any $p$, the string becomes $5$-proper.</p>
