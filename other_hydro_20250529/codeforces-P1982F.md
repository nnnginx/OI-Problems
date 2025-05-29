## Description

<div><p>You have an array $a$ of $n$ elements. There are also $q$ modifications of the array. Before the first modification and after each modification, you would like to know the following:</p><p>What is the minimum length subarray that needs to be sorted in non-decreasing order in order for the array $a$ to be completely sorted in non-decreasing order?</p><p>More formally, you want to select a subarray of the array $(l, r)$ with the minimum value of $r - l + 1$. After that, you will sort the elements $a_{l}, a_{l + 1}, \ldots, a_{r}$ and want the condition $a_{i} \le a_{i + 1}$ to hold for all $1 \le i &lt; n$. If the array is already sorted in non-decreasing order, then $l$ and $r$ should be considered as equal to $-1$.</p><p>Note that finding such $(l, r)$ does not change the array in any way. The modifications themselves take the form: assign $a_{pos} = x$ for given $pos$ and $x$.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;！ the number of test cases. Then follows the description of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^{5}$).</p><p>The second line of each test case contains $n$ integers $a_{i}$ ($0 \le |a_{i}| \le 10^{9}$)&nbsp;！ the initial elements of the array $a$.</p><p>The third line of each test case contains a number $q$ ($0 \le q \le 5 \cdot 10^{5}$)&nbsp;！ the number of modifications to the array.</p><p>The following $q$ lines of each test case contain two integers $pos_{i}$ ($1 \le pos_{i} \le n$) and $val_{i}$ ($0 \le |val_{i}| \le 10^{9}$)&nbsp;！ this means that for the $i$-th modification, $a_{pos_{i}}$ is assigned the value $val_{i}$.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ for all test cases does not exceed $5 \cdot 10^{5}$.</p></div><div class="output-specification"><p>For each test case, output $q + 1$ lines. Each line should contain $2$ integers $l, r$&nbsp;！ the boundaries of the minimum subarray, such that sorting it will make the array $a$ completely sorted. If $a$ is already sorted, then output $l = -1$, $r = -1$.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10$)&nbsp;！ the number of test cases. Then follows the description of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^{5}$).</p><p>The second line of each test case contains $n$ integers $a_{i}$ ($0 \le |a_{i}| \le 10^{9}$)&nbsp;！ the initial elements of the array $a$.</p><p>The third line of each test case contains a number $q$ ($0 \le q \le 5 \cdot 10^{5}$)&nbsp;！ the number of modifications to the array.</p><p>The following $q$ lines of each test case contain two integers $pos_{i}$ ($1 \le pos_{i} \le n$) and $val_{i}$ ($0 \le |val_{i}| \le 10^{9}$)&nbsp;！ this means that for the $i$-th modification, $a_{pos_{i}}$ is assigned the value $val_{i}$.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ for all test cases does not exceed $5 \cdot 10^{5}$.</p>

## Output

<p>For each test case, output $q + 1$ lines. Each line should contain $2$ integers $l, r$&nbsp;！ the boundaries of the minimum subarray, such that sorting it will make the array $a$ completely sorted. If $a$ is already sorted, then output $l = -1$, $r = -1$.</p>





```input1|2,3,4,5,6,7
2
5
2 2 3 4 5
3
2 1
4 1
1 1
5
1 2 3 4 5
9
1 4
2 3
5 2
3 1
1 1
5 1
4 1
3 1
2 1
```




```output1
-1 -1
1 2
1 4
3 4
-1 -1
1 3
1 3
1 5
1 5
2 5
2 5
2 5
2 5
-1 -1
```



## Note

<p>Let's consider the first test case:</p><ul> <li> Initially, the array is sorted in non-decreasing order: $[2, 2, 3, 4, 5]$ </li><li> After the first query, the array looks like this: $[\color{red}{2}, \color{red}{1}, 3, 4, 5]$. </li><li> After the second query, the array looks like this: $[\color{red}{2}, \color{red}{1}, \color{red}{3}, \color{red}{1}, 5]$. </li><li> After the third query, the array looks like this: $[1, 1, \color{red}{3}, \color{red}{1}, 5]$. </li></ul><p>The red segments indicate the subarrays that need to be sorted in order for the entire array to be sorted in non-decreasing order.</p>
