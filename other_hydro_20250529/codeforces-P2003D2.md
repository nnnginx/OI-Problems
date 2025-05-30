## Description

<div><p><span class="tex-font-style-bf">The two versions are different problems. In this version of the problem, you can't choose the same integer twice or more. You can make hacks only if both versions are solved.</span></p><p>One day, Turtle was playing with $n$ sequences. Let the length of the $i$-th sequence be $l_i$. Then the $i$-th sequence was $a_{i, 1}, a_{i, 2}, \ldots, a_{i, l_i}$.</p><p>Piggy gave Turtle a problem to solve when Turtle was playing. The statement of the problem was:</p><ul> <li> There was a non-negative integer $x$ at first. Turtle would perform an arbitrary number (possibly zero) of operations on the integer. </li><li> In each operation, Turtle could choose an integer $i$ such that $1 \le i \le n$ and <span class="tex-font-style-bf">$i$ wasn't chosen before</span>, and set $x$ to $\text{mex}^{\dagger}(x, a_{i, 1}, a_{i, 2}, \ldots, a_{i, l_i})$. </li><li> Turtle was asked to find the answer, which was the <span class="tex-font-style-bf">maximum</span> value of $x$ after performing an arbitrary number of operations. </li></ul><p>Turtle solved the above problem without difficulty. He defined $f(k)$ as the answer to the above problem when the initial value of $x$ was $k$.</p><p>Then Piggy gave Turtle a non-negative integer $m$ and asked Turtle to find the value of $\sum\limits_{i = 0}^m f(i)$ (i.e., the value of $f(0) + f(1) + \ldots + f(m)$). Unfortunately, he couldn't solve this problem. Please help him!</p><p>$^{\dagger}\text{mex}(c_1, c_2, \ldots, c_k)$ is defined as the smallest <span class="tex-font-style-bf">non-negative</span> integer $x$ which does not occur in the sequence $c$. For example, $\text{mex}(2, 2, 0, 3)$ is $1$, $\text{mex}(1, 2)$ is $0$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($1 \le n \le 2 \cdot 10^5, 0 \le m \le 10^9$).</p><p>Each of the following $n$ lines contains several integers. The first integer $l_i$ ($1 \le l_i \le 2 \cdot 10^5$) represents the length of the $i$-th sequence, and the following $l_i$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, l_i}$ ($0 \le a_{i, j} \le 10^9$) represent the elements of the $i$-th sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $\sum l_i$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the value of $\sum\limits_{i = 0}^m f(i)$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($1 \le n \le 2 \cdot 10^5, 0 \le m \le 10^9$).</p><p>Each of the following $n$ lines contains several integers. The first integer $l_i$ ($1 \le l_i \le 2 \cdot 10^5$) represents the length of the $i$-th sequence, and the following $l_i$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, l_i}$ ($0 \le a_{i, j} \le 10^9$) represent the elements of the $i$-th sequence.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$ and the sum of $\sum l_i$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer �� the value of $\sum\limits_{i = 0}^m f(i)$.</p>





```input1|2,3,4,5,10,11,12,15,16,17,18,19
6
3 4
2 0 2
3 2 3 3
4 7 0 1 5
3 4
5 0 2 0 4 11
1 1
5 1 3 0 3 3
2 50
2 1 2
2 1 2
1 1
7 1 2 4 1 4 9 5
4 114514
2 2 2
5 7 3 6 0 3
3 0 1 1
5 0 9 2 1 5
5 1919810
1 2
2 324003 0
3 1416324 2 1460728
4 1312631 2 0 1415195
5 1223554 192248 2 1492515 725556
```




```output1
16
18
1281
4
6556785365
1842836177961
```



## Note

<p>In the first test case, when $x$ is initially $2$, Turtle can choose $i = 3$ and set $x$ to $\text{mex}(x, a_{3, 1}, a_{3, 2}, a_{3, 3}, a_{3, 4}) = \text{mex}(2, 7, 0, 1, 5) = 3$. It can be proved that Turtle can't make the value of $x$ greater than $3$, so $f(2) = 3$.</p><p>It can be seen that $f(0) = 3$, $f(1) = 3$, $f(2) = 3$, $f(3) = 3$, and $f(4) = 4$. So $f(0) + f(1) + f(2) + f(3) + f(4) = 3 + 3 + 3 + 3 + 4 = 16$.</p><p>In the second test case, when $x$ is initially $1$, Turtle can choose $i = 1$ and set $x$ to $\text{mex}(x, a_{1, 1}, a_{1, 2}, a_{1, 3}, a_{1, 4}, a_{1, 5}) = \text{mex}(1, 0, 2, 0, 4, 11) = 3$. It can be proved that Turtle can't make the value of $x$ greater than $3$, so $f(1) = 3$.</p><p>It can be seen that $f(0) = 4$, $f(1) = 3$, $f(2) = 4$, $f(3) = 3$, and $f(4) = 4$. So $f(0) + f(1) + f(2) + f(3) + f(4) = 4 + 3 + 4 + 3 + 4 = 18$.</p><p>In the fourth test case, it can be seen that $f(0) = 3$ and $f(1) = 1$. So $f(0) + f(1) = 3 + 1 = 4$.</p>
