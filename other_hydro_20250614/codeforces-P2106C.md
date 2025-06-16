## Description

<div><p>Two integer arrays $a$ and $b$ of size $n$ are <span class="tex-font-style-bf">complementary</span> if there exists an integer $x$ such that $a_i + b_i = x$ over all $1 \le i \le n$. For example, the arrays $a = [2, 1, 4]$ and $b = [3, 4, 1]$ are complementary, since $a_i + b_i = 5$ over all $1 \le i \le 3$. However, the arrays $a = [1, 3]$ and $b = [2, 1]$ are not complementary.</p><p>Cow the Nerd thinks everybody is interested in math, so he gave Cherry Bomb two integer arrays $a$ and $b$. It is known that $a$ and $b$ both contain $n$ <span class="tex-font-style-bf">non-negative</span> integers not greater than $k$. </p><p>Unfortunately, Cherry Bomb has lost some elements in $b$. Lost elements in $b$ are denoted with $-1$. Help Cherry Bomb count the number of possible arrays $b$ such that:</p><ul> <li> $a$ and $b$ are <span class="tex-font-style-bf">complementary</span>. </li><li> All lost elements are replaced with non-negative integers no more than $k$. </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$)&nbsp;！ the size of the arrays and the maximum possible value of their elements.</p><p>The second line contains $n$ integers $a_1, a_2, ..., a_n$ ($0 \le a_i \le k$).</p><p>The third line contains $n$ integers $b_1, b_2, ..., b_n$ ($-1 \le b_i \le k$). If $b_i = -1$, then this element is missing.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output exactly one integer, the number of ways Cherry Bomb can fill in the missing elements from $b$ such that $a$ and $b$ are complementary.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $0 \le k \le 10^9$)&nbsp;！ the size of the arrays and the maximum possible value of their elements.</p><p>The second line contains $n$ integers $a_1, a_2, ..., a_n$ ($0 \le a_i \le k$).</p><p>The third line contains $n$ integers $b_1, b_2, ..., b_n$ ($-1 \le b_i \le k$). If $b_i = -1$, then this element is missing.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output exactly one integer, the number of ways Cherry Bomb can fill in the missing elements from $b$ such that $a$ and $b$ are complementary.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
3 10
1 3 2
-1 -1 1
5 1
0 1 0 0 1
-1 0 1 0 -1
5 1
0 1 0 0 1
-1 1 -1 1 -1
5 10
1 3 2 5 4
-1 -1 -1 -1 -1
5 4
1 3 2 1 3
1 -1 -1 1 -1
5 4
1 3 2 1 3
2 -1 -1 2 0
5 5
5 0 5 4 3
5 -1 -1 -1 -1
```




```output1
1
0
0
7
0
1
0
```



## Note

<p>In the first example, the only way to fill in the missing elements in $b$ such that $a$ and $b$ are complementary is if $b = [2, 0, 1]$.</p><p>In the second example, there is no way to fill in the missing elements of $b$ such that $a$ and $b$ are complementary.</p><p>In the fourth example, some $b$ arrays that are complementary to $a$ are: $[4, 2, 3, 0, 1], [7, 5, 6, 3, 4],$ and $[9, 7, 8, 5, 6]$.</p>
