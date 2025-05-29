## Description

<div><p>Bob decided to open a bakery. On the opening day, he baked $n$ buns that he can sell. The usual price of a bun is $a$ coins, but to attract customers, Bob organized the following promotion:</p><ul><li> Bob chooses some integer $k$ ($0 \le k \le \min(n, b)$).</li><li> Bob sells the first $k$ buns at a modified price. In this case, the price of the $i$-th ($1 \le i \le k$) sold bun is $(b - i + 1)$ coins.</li><li> The remaining $(n - k)$ buns are sold at $a$ coins each.</li></ul><p>Note that $k$ can be equal to $0$. In this case, Bob will sell all the buns at $a$ coins each.</p><p>Help Bob determine the maximum profit he can obtain by selling all $n$ buns.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$, and $b$ ($1 \le n, a, b \le 10^9$)&nbsp;！ the number of buns, the usual price of a bun, and the price of the first bun to be sold at a modified price.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the maximum profit that Bob can obtain.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$, and $b$ ($1 \le n, a, b \le 10^9$)&nbsp;！ the number of buns, the usual price of a bun, and the price of the first bun to be sold at a modified price.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the maximum profit that Bob can obtain.</p>





```input1|2,4,6,8
7
4 4 5
5 5 9
10 10 5
5 5 11
1000000000 1000000000 1000000000
1000000000 1000000000 1
1000 1 1000
```




```output1
17
35
100
45
1000000000000000000
1000000000000000000
500500
```



## Note

<p>In the first test case, it is optimal for Bob to choose $k = 1$. Then he will sell one bun for $5$ coins, and three buns at the usual price for $4$ coins each. Then the profit will be $5 + 4 + 4 + 4 = 17$ coins.</p><p>In the second test case, it is optimal for Bob to choose $k = 5$. Then he will sell all the buns at the modified price and obtain a profit of $9 + 8 + 7 + 6 + 5 = 35$ coins.</p><p>In the third test case, it is optimal for Bob to choose $k = 0$. Then he will sell all the buns at the usual price and obtain a profit of $10 \cdot 10 = 100$ coins.</p>
