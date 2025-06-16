## Description

<div><p>You are given an array $x_2,x_3,\dots,x_n$. Your task is to find <span class="tex-font-style-bf">any</span> array $a_1,\dots,a_n$, where: </p><ul> <li> $1\le a_i\le 10^9$ for all $1\le i\le n$. </li><li> $x_i=a_i \bmod a_{i-1}$ for all $2\le i\le n$. </li></ul><p>Here $c\bmod d$ denotes the remainder of the division of the integer $c$ by the integer $d$. For example $5 \bmod 2 = 1$, $72 \bmod 3 = 0$, $143 \bmod 14 = 3$.</p><p><span class="tex-font-style-bf">Note that if there is more than one $a$ which satisfies the statement, you are allowed to find any.</span></p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1\le t\le 10^4)$&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 500)$&nbsp;！ the number of elements in $a$.</p><p>The second line of each test case contains $n-1$ integers $x_2,\dots,x_n$ $(1\le x_i\le 500)$&nbsp;！ the elements of $x$.</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output any $a_1,\dots,a_n$ ($1 \le a_i \le 10^9$) which satisfies the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1\le t\le 10^4)$&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(2\le n\le 500)$&nbsp;！ the number of elements in $a$.</p><p>The second line of each test case contains $n-1$ integers $x_2,\dots,x_n$ $(1\le x_i\le 500)$&nbsp;！ the elements of $x$.</p><p>It is guaranteed that the sum of values $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output any $a_1,\dots,a_n$ ($1 \le a_i \le 10^9$) which satisfies the statement.</p>





```input1|2,3,6,7,10,11
5
4
2 4 1
3
1 1
6
4 2 5 1 2
2
500
3
1 5
```




```output1
3 5 4 9
2 5 11
5 14 16 5 11 24
501 500
2 7 5
```



## Note

<p>In the first test case $a=[3,5,4,9]$ satisfies the conditions, because: </p><ul> <li> $a_2\bmod a_1=5\bmod 3=2=x_2$; </li><li> $a_3\bmod a_2=4\bmod 5=4=x_3$; </li><li> $a_4\bmod a_3=9\bmod 4=1=x_4$; </li></ul>
