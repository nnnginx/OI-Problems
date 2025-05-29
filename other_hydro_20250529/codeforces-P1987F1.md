## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The only difference between the two versions is the constraint on $n$. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given an array of integers $a$ of length $n$. </p><p>In one operation, you will perform the following two-step process: </p><ol> <li> Choose an index $i$ such that $1 \le i &lt; |a|$ and $a_i = i$. </li><li> Remove $a_i$ and $a_{i+1}$ from the array and concatenate the remaining parts. </li></ol><p>Find the maximum number of times that you can perform the operation above.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the maximum number of times that you can perform the operation.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;！ the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;！ the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the maximum number of times that you can perform the operation.</p>





```input1|2,3,6,7,10,11
6
5
1 5 3 2 4
8
2 1 3 4 5 6 7 8
3
1 2 3
4
1 2 4 4
5
4 4 1 3 5
1
1
```




```output1
2
3
1
2
0
0
```



## Note

<p>In the first test case, one possible optimal sequence of operations is $[ 1, 5, \color{red}{3}, \color{red}{2}, 4 ] \rightarrow [\color{red}{1}, \color{red}{5}, 4] \rightarrow [4]$.</p><p>In the third test case, one possible optimal sequence of operations is $[1, \color{red}{2}, \color{red}{3}] \rightarrow [1]$.</p>
