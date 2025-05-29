## Description

<div><p>Given two arrays of distinct positive integers $a$ and $b$ of length $n$, we would like to make both the arrays the same. Two arrays $x$ and $y$ of length $k$ are said to be the same when for all $1 \le i \le k$, $x_i = y_i$.</p><p>Now in one move, you can choose some index $l$ and $r$ in $a$ ($l \le r$) and swap $a_l$ and $a_r$, then choose some $p$ and $q$ ($p \le q$) in $b$ such that $r-l=q-p$ and swap $b_p$ and $b_q$.</p><p>Is it possible to make both arrays the same?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ distinct integers $a_1,a_2,a_3,\ldots,a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the integers in the array $a$.</p><p>The third line of each test case contains $n$ distinct integers $b_1,b_2,b_3,\ldots,b_n$ ($1 \le b_i \le 2 \cdot 10^5$)&nbsp;！ the integers in the array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the arrays $a$ and $b$ can be made the same. Otherwise, print "<span class="tex-font-style-tt">NO</span>". can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2 \cdot 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ distinct integers $a_1,a_2,a_3,\ldots,a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the integers in the array $a$.</p><p>The third line of each test case contains $n$ distinct integers $b_1,b_2,b_3,\ldots,b_n$ ($1 \le b_i \le 2 \cdot 10^5$)&nbsp;！ the integers in the array $b$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if the arrays $a$ and $b$ can be made the same. Otherwise, print "<span class="tex-font-style-tt">NO</span>". can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,8,9,10,14,15,16
6
4
1 2 3 4
1 2 3 4
5
1 3 4 2 5
7 1 2 5 4
4
1 2 3 4
4 3 2 1
3
1 2 3
1 3 2
5
1 5 7 1000 4
4 1 7 5 1000
3
1 4 2
1 3 2
```




```output1
YES
NO
YES
NO
NO
NO
```



## Note

<p>In the first testcase, you don't need to perform any operations since the arrays are same.</p><p>In the second testcase, it can be proven there exists no way to make the arrays same.</p><p>In the third testcase, one of the ways to make the arrays same is to first choose $l=1$, $r=3$, $p=1$, $q=3$ then choose $l=1$, $r=2$, $p=3$, $q=4$.</p>
