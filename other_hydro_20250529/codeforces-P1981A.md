## Description

<div><p>Turtle and Piggy are playing a number game.</p><p>First, Turtle will choose an integer $x$, such that $l \le x \le r$, where $l, r$ are given. It's also guaranteed that $2l \le r$.</p><p>Then, Piggy will keep doing the following operation until $x$ becomes $1$:</p><ul> <li> Choose an integer $p$ such that $p \ge 2$ and $p \mid x$ (i.e. $x$ is a multiple of $p$). </li><li> Set $x$ to $\frac{x}{p}$, and the score will increase by $1$. </li></ul><p>The score is initially $0$. Both Turtle and Piggy want to maximize the score. Please help them to calculate the maximum score.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $l, r$ ($1 \le l \le r \le 10^9, 2l \le r$) ！ The range where Turtle can choose the integer from.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the maximum score.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $l, r$ ($1 \le l \le r \le 10^9, 2l \le r$) ！ The range where Turtle can choose the integer from.</p>

## Output

<p>For each test case, output a single integer ！ the maximum score.</p>





```input1|2,4,6
5
2 4
3 6
2 15
6 22
114514 1919810
```




```output1
2
2
3
4
20
```



## Note

<p>In the first test case, Turtle can choose an integer $x$, such that $2 \le x \le 4$. He can choose $x = 4$. Then Piggy can choose $p = 2$ for $2$ times. After that, $x$ will become $1$, and the score will be $2$, which is maximized.</p><p>In the second test case, Turtle can choose an integer $3 \le x \le 6$. He can choose $x = 6$. Then Piggy can choose $p = 2$, then choose $p = 3$. After that, $x$ will become $1$, and the score will be $2$, which is maximum.</p><p>In the third test case, Turtle can choose $x = 12$.</p><p>In the fourth test case, Turtle can choose $x = 16$.</p>
