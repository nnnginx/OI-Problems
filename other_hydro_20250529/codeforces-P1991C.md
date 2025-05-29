## Description

<div><p>You are given an array $a$ of $n$ integers.</p><p>In one operation, you will perform the following two-step move: </p><ol> <li> Choose an integer $x$ ($0 \le x \le 10^{9}$). </li><li> Replace each $a_i$ with $|a_i - x|$, where $|v|$ denotes the <a href="https://en.wikipedia.org/wiki/Absolute_value">absolute value</a> of $v$. </li></ol><p>For example, by choosing $x = 8$, the array $[5, 7, 10]$ will be changed into $[|5-8|, |7-8|, |10-8|] = [3,1,2]$.</p><p>Construct a sequence of operations to make all elements of $a$ equal to $0$ in at most $40$ operations or determine that it is impossible. You do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer $-1$ if it is impossible to make all array elements equal to $0$ in at most $40$ operations.</p><p>Otherwise, output two lines. The first line of output should contain a single integer $k$ ($0 \le k \le 40$)&nbsp;！ the number of operations. The second line of output should contain $k$ integers $x_1, x_2, \ldots, x_k$ ($0 \le x_i \le 10^{9}$)&nbsp;！ the sequence of operations, denoting that on the $i$-th operation, you chose $x=x_i$.</p><p>If there are multiple solutions, output any of them.</p><p>You do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer $-1$ if it is impossible to make all array elements equal to $0$ in at most $40$ operations.</p><p>Otherwise, output two lines. The first line of output should contain a single integer $k$ ($0 \le k \le 40$)&nbsp;！ the number of operations. The second line of output should contain $k$ integers $x_1, x_2, \ldots, x_k$ ($0 \le x_i \le 10^{9}$)&nbsp;！ the sequence of operations, denoting that on the $i$-th operation, you chose $x=x_i$.</p><p>If there are multiple solutions, output any of them.</p><p>You do <span class="tex-font-style-bf">not</span> need to minimize the number of operations.</p>





```input1|2,3,6,7,10,11
5
1
5
2
0 0
3
4 6 8
4
80 40 20 10
5
1 2 3 4 5
```




```output1
1
5
0

3
6 1 1
7
60 40 20 10 30 25 5
-1
```



## Note

<p>In the first test case, we can perform only one operation by choosing $x = 5$, changing the array from $[5]$ to $[0]$.</p><p>In the second test case, no operations are needed because all elements of the array are already $0$.</p><p>In the third test case, we can choose $x = 6$ to change the array from $[4, 6, 8]$ to $[2, 0, 2]$, then choose $x = 1$ to change it to $[1, 1, 1]$, and finally choose $x = 1$ again to change the array into $[0, 0, 0]$.</p><p>In the fourth test case, we can make all elements $0$ by following the operation sequence $(60, 40, 20, 10, 30, 25, 5)$.</p><p>In the fifth test case, it can be shown that it is impossible to make all elements $0$ in at most $40$ operations. Therefore, the output is $-1$.</p>
