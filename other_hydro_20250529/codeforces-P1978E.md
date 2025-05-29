## Description

<div><p>Sasha has two binary strings $s$ and $t$ of the same length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>There is also a computing machine that can perform two types of operations on binary strings $a$ and $b$ of the same length $k$:</p><ol> <li> If $a_{i} = a_{i + 2} =$ <span class="tex-font-style-tt">0</span>, then you can assign $b_{i + 1} :=$ <span class="tex-font-style-tt">1</span> ($1 \le i \le k - 2$). </li><li> If $b_{i} = b_{i + 2} =$ <span class="tex-font-style-tt">1</span>, then you can assign $a_{i + 1} :=$ <span class="tex-font-style-tt">1</span> ($1 \le i \le k - 2$). </li></ol><p>Sasha became interested in the following: if we consider the string $a=s_ls_{l+1}\ldots s_r$ and the string $b=t_lt_{l+1}\ldots t_r$, what is the maximum number of <span class="tex-font-style-tt">1</span> characters in the string $a$ that can be obtained using the computing machine. Since Sasha is very curious but lazy, it is up to you to answer this question for several pairs $(l_i, r_i)$ that interest him.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{4}$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the strings $s$ and $t$.</p><p>The second line of each test case contains a binary string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line of each test case contains a binary string $t$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The fourth line of each test case contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>The $i$-th of the following lines contains two integers $l_{i}$ and $r_{i}$ ($1 \le l_{i} \le r_{i} \le n$) ！ the boundaries of the $i$-th pair of substrings that interest Sasha.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $q$ integers ！ the answers to all queries.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^{4}$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the strings $s$ and $t$.</p><p>The second line of each test case contains a binary string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line of each test case contains a binary string $t$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The fourth line of each test case contains a single integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries.</p><p>The $i$-th of the following lines contains two integers $l_{i}$ and $r_{i}$ ($1 \le l_{i} \le r_{i} \le n$) ！ the boundaries of the $i$-th pair of substrings that interest Sasha.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $q$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output $q$ integers ！ the answers to all queries.</p>





```input1|2,3,4,5,6,7,14,15,16,17,18,19,20,21,22
3
4
1111
0000
2
1 2
2 4
4
1010
1101
2
1 3
1 4
6
010101
011010
5
2 3
1 6
2 5
4 4
3 6
```




```output1
2
3
2
3
1
4
3
1
2
```



## Note

<p>In the first test case: </p><ul> <li> In the first query, $a =$ <span class="tex-font-style-tt">11</span>, so the maximum number of <span class="tex-font-style-tt">1</span> characters is $2$. </li><li> In the second query, $a =$ <span class="tex-font-style-tt">111</span>, so the maximum number of <span class="tex-font-style-tt">1</span> characters is $3$. </li></ul><p>In the second test case: </p><ul> <li> In the first query, $a =$ <span class="tex-font-style-tt">101</span> and $b =$ <span class="tex-font-style-tt">110</span>. No operations can be performed, so the maximum number of <span class="tex-font-style-tt">1</span> characters is $2$. </li><li> In the second query, $a =$ <span class="tex-font-style-tt">1010</span> and $b =$ <span class="tex-font-style-tt">1101</span>. Since $a_2 = a_4 =$ <span class="tex-font-style-tt">0</span>, we can assign $b_3 :=$ <span class="tex-font-style-tt">1</span>. Now $b_1 = b_3 =$ <span class="tex-font-style-tt">1</span>, so we can assign $a_2 :=$ <span class="tex-font-style-tt">1</span>. The string $a$ becomes <span class="tex-font-style-tt">1110</span>, so the maximum number of <span class="tex-font-style-tt">1</span> characters is $3$. </li></ul>
