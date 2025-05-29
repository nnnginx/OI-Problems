## Description

<div><p>Let us call an array $x_1,\dots,x_m$ interesting if it is possible to divide the array into $k&gt;1$ parts so that <a href="http://tiny.cc/xor_wiki_eng">bitwise XOR</a> of values from each part are equal. </p><p>More formally, you must split array $x$ into $k$ consecutive segments, each element of $x$ must belong to <span class="tex-font-style-bf">exactly</span> $1$ segment. Let $y_1,\dots,y_k$ be the XOR of elements from each part respectively. Then $y_1=y_2=\dots=y_k$ must be fulfilled.</p><p>For example, if $x = [1, 1, 2, 3, 0]$, you can split it as follows: $[\color{blue}1], [\color{green}1], [\color{red}2, \color{red}3, \color{red}0]$. Indeed $\color{blue}1=\color{green}1=\color{red}2 \oplus \color{red}3\oplus \color{red}0$.</p><p>You are given an array $a_1,\dots,a_n$. Your task is to answer $q$ queries: </p><ul> <li> For fixed $l$, $r$, determine whether the subarray $a_l,a_{l+1},\dots,a_r$ is interesting. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($2 \le n \le 2 \cdot 10^5$, $1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of elements in the array and the number of queries respectively.</p><p>The next line contains $n$ integers $a_1,\dots,a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ elements of the array.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$) describing the query.</p><p>It is guaranteed that the sum of $n$ over all testcases does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of $q$ over all testcases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each query, output "<span class="tex-font-style-tt">YES</span>" if the subarray is interesting and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as correct answers).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $q$ ($2 \le n \le 2 \cdot 10^5$, $1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of elements in the array and the number of queries respectively.</p><p>The next line contains $n$ integers $a_1,\dots,a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;！ elements of the array.</p><p>Each of the next $q$ lines contains two integers $l$ and $r$ ($1 \le l &lt; r \le n$) describing the query.</p><p>It is guaranteed that the sum of $n$ over all testcases does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the sum of $q$ over all testcases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each query, output "<span class="tex-font-style-tt">YES</span>" if the subarray is interesting and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, the strings "<span class="tex-font-style-tt">yES</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as correct answers).</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,20,21
4
5 5
1 1 2 3 0
1 5
2 4
3 5
1 3
3 4
5 5
1 2 3 4 5
1 5
2 4
3 5
1 3
2 3
7 4
12 9 10 9 10 11 9
1 5
1 7
2 6
2 7
11 4
0 0 1 0 0 1 0 1 1 0 1
1 2
2 5
6 9
7 11
```




```output1
YES
YES
NO
NO
NO

YES
NO
NO
YES
NO

NO
NO
NO
NO

YES
NO
YES
YES
```



## Note

<p>Explanation for the first test case:</p><p>The first query is described in the statement.</p><p>In the second query, we should divide $[1,2,3]$. A possible division is $[1,2],[3]$, since $1\oplus 2=3$.</p><p>It can be shown that for queries $3,4,5$, the subarrays are not interesting.</p>
