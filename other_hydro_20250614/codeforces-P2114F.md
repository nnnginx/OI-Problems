## Description

<div><p>Given an integer $x$ and an integer $k$. In one operation, you can perform one of two actions:</p><ul> <li> choose an integer $1 \le a \le k$ and assign $x = x \cdot a$; </li><li> choose an integer $1 \le a \le k$ and assign $x = \frac{x}{a}$, where the value of $\frac{x}{a}$ must be an integer. </li></ul><p>Find the minimum number of operations required to make the number $x$ equal to $y$, or determine that it is impossible.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains three integers $x$, $y$ and $k$ ($1 \le x, y, k \le 10^6$).</p><p>It is guaranteed that the sum of $x$ and the sum of $y$ across all test cases does not exceed $10^8$.</p></div><div class="output-specification"><p>For each test case, output $-1$ if it is impossible to achieve $x=y$ using the given operations, and the minimum number of required operations otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;¡ª the number of test cases.</p><p>The only line of each test case contains three integers $x$, $y$ and $k$ ($1 \le x, y, k \le 10^6$).</p><p>It is guaranteed that the sum of $x$ and the sum of $y$ across all test cases does not exceed $10^8$.</p>

## Output

<p>For each test case, output $-1$ if it is impossible to achieve $x=y$ using the given operations, and the minimum number of required operations otherwise.</p>





```input1|2,4,6,8
8
4 6 3
4 5 3
4 6 2
10 45 3
780 23 42
11 270 23
1 982800 13
1 6 2
```




```output1
2
-1
-1
3
3
3
6
-1
```


