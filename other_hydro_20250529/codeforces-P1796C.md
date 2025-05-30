## Description

<div><p>A set of positive integers $S$ is called beautiful if, for every two integers $x$ and $y$ from this set, either $x$ divides $y$ or $y$ divides $x$ (or both).</p><p>You are given two integers $l$ and $r$. Consider all beautiful sets consisting of integers not less than $l$ and not greater than $r$. You have to print two numbers:</p><ul> <li> the maximum possible size of a beautiful set where all elements are from $l$ to $r$; </li><li> the number of beautiful sets consisting of integers from $l$ to $r$ with the maximum possible size. </li></ul><p>Since the second number can be very large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases.</p><p>Each test case consists of one line containing two integers $l$ and $r$ ($1 \le l \le r \le 10^6$).</p></div><div class="output-specification"><p>For each test case, print two integers �� the maximum possible size of a beautiful set consisting of integers from $l$ to $r$, and the number of such sets with maximum possible size. Since the second number can be very large, print it modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases.</p><p>Each test case consists of one line containing two integers $l$ and $r$ ($1 \le l \le r \le 10^6$).</p>

## Output

<p>For each test case, print two integers �� the maximum possible size of a beautiful set consisting of integers from $l$ to $r$, and the number of such sets with maximum possible size. Since the second number can be very large, print it modulo $998244353$.</p>





```input1|2,4
4
3 11
13 37
1 22
4 100
```




```output1
2 4
2 6
5 1
5 7
```



## Note

<p>In the first test case, the maximum possible size of a beautiful set with integers from $3$ to $11$ is $2$. There are $4$ such sets which have the maximum possible size:</p><ul> <li> $\{ 3, 6 \}$; </li><li> $\{ 3, 9 \}$; </li><li> $\{ 4, 8 \}$; </li><li> $\{ 5, 10 \}$. </li></ul>
