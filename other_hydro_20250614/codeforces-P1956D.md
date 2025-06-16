## Description

<div><p>Nene gave you an array of integers $a_1, a_2, \ldots, a_n$ of length $n$.</p><p>You can perform the following operation no more than $5\cdot 10^5$ times (possibly zero):</p><ul> <li> Choose two integers $l$ and $r$ such that $1 \le l \le r \le n$, compute $x$ as $\operatorname{MEX}(\{a_l, a_{l+1}, \ldots, a_r\})$, and simultaneously set $a_l:=x, a_{l+1}:=x, \ldots, a_r:=x$. </li></ul><p>Here, $\operatorname{MEX}$ of a set of integers $\{c_1, c_2, \ldots, c_k\}$ is defined as the smallest non-negative integer $m$ which does not occur in the set $c$.</p><p>Your goal is to maximize the sum of the elements of the array $a$. Find the maximum sum and construct a sequence of operations that achieves this sum. Note that you don't need to minimize the number of operations in this sequence, you only should use no more than $5\cdot 10^5$ operations in your solution.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 18$)&nbsp;！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\leq a_i \leq 10^7$)&nbsp;！ the array $a$.</p></div><div class="output-specification"><p>In the first line, output two integers $s$ and $m$ ($0\le m\le 5\cdot 10^5$)&nbsp;！ the maximum sum of elements of the array $a$ and the number of operations in your solution.</p><p>In the $i$-th of the following $m$ lines, output two integers $l$ and $r$ ($1 \le l \le r \le n$), representing the parameters of the $i$-th operation.</p><p>It can be shown that the maximum sum of elements of the array $a$ can always be obtained in no more than $5 \cdot 10^5$ operations.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 18$)&nbsp;！ the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\leq a_i \leq 10^7$)&nbsp;！ the array $a$.</p>

## Output

<p>In the first line, output two integers $s$ and $m$ ($0\le m\le 5\cdot 10^5$)&nbsp;！ the maximum sum of elements of the array $a$ and the number of operations in your solution.</p><p>In the $i$-th of the following $m$ lines, output two integers $l$ and $r$ ($1 \le l \le r \le n$), representing the parameters of the $i$-th operation.</p><p>It can be shown that the maximum sum of elements of the array $a$ can always be obtained in no more than $5 \cdot 10^5$ operations.</p>





```input1|
2
0 1
```




```input2|
3
1 3 9
```




```input3|
4
1 100 2 1
```




```input4|
1
0
```




```output1
4 1
1 2
```




```output2
13 0
```




```output3
105 2
3 3
3 4
```




```output4
1 1
1 1
```



## Note

<p>In the first example, after the operation with $l=1$ and $r=2$ the array $a$ becomes equal to $[2,2]$. It can be shown that it is impossible to achieve a larger sum of the elements of $a$, so the answer is $4$.</p><p>In the second example, the initial sum of elements is $13$ which can be shown to be the largest.</p><p>In the third example, the array $a$ changes as follows:</p><ul> <li> after the first operation ($l=3$, $r=3$), the array $a$ becomes equal to $[1,100,0,1]$; </li><li> after the second operation ($l=3$, $r=4$), the array $a$ becomes equal to $[1,100,2,2]$. </li></ul><p>It can be shown that it is impossible to achieve a larger sum of the elements of $a$, so the answer is $105$.</p>
