## Description

<div><p>We define the $\operatorname{MAD}$ (Maximum Appearing Duplicate) in an array as the largest number that appears at least twice in the array. Specifically, if there is no number that appears at least twice, the $\operatorname{MAD}$ value is $0$.</p><p>For example, $\operatorname{MAD}([1, 2, 1]) = 1$, $\operatorname{MAD}([2, 2, 3, 3]) = 3$, $\operatorname{MAD}([1, 2, 3, 4]) = 0$.</p><p>You are given an array $a$ of size $n$. Initially, a variable $sum$ is set to $0$.</p><p>The following process will be executed in a sequential loop until all numbers in $a$ become $0$:</p><ol> <li> Set $sum := sum + \sum_{i=1}^{n} a_i$; </li><li> Let $b$ be an array of size $n$. Set $b_i :=\ \operatorname{MAD}([a_1, a_2, \ldots, a_i])$ for all $1 \le i \le n$, and then set $a_i := b_i$ for all $1 \le i \le n$. </li></ol><p>Find the value of $sum$ after the process.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the size of the array $a$; </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;！ the elements of the array. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the value of $sum$ in a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 2 \cdot 10^4$)&nbsp;！ the number of test cases.</p><p>For each test case: </p><ul> <li> The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$)&nbsp;！ the size of the array $a$; </li><li> The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$)&nbsp;！ the elements of the array. </li></ul><p>It is guaranteed that the sum of $n$ over all test cases will not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the value of $sum$ in a new line.</p>





```input1|2,3,6,7
4
1
1
3
2 2 3
4
2 1 1 2
4
4 4 4 4
```




```output1
1
13
9
40
```



## Note

<p>In the first test case, $a=[1]$ initially.</p><p>In the first loop: </p><ol> <li> Set $sum := sum + a_1 = 0+1=1$; </li><li> Set $b_1 :=\ \operatorname{MAD}([a_1])=\ \operatorname{MAD}([1])=0$, and then set $a_1 := b_1$. </li></ol><p>After the first loop, $a=[0]$ and the process ends. The value of $sum$ after the process is $1$.</p><p>In the second test case, $a=[2,2,3]$ initially.</p><p>After the first loop, $a=[0,2,2]$ and $sum=7$.</p><p>After the second loop, $a=[0,0,2]$ and $sum=11$.</p><p>After the third loop, $a=[0,0,0]$ and $sum=13$. Then the process ends.</p><p>The value of $sum$ after the process is $13$.</p>
