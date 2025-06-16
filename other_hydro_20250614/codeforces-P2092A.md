## Description

<div><p>Kamilka has a flock of $n$ sheep, the $i$-th of which has a beauty level of $a_i$. All $a_i$ are distinct. Morning has come, which means they need to be fed. Kamilka can choose a non-negative integer $d$ and give each sheep $d$ bunches of grass. After that, the beauty level of each sheep increases by $d$.</p><p>In the evening, Kamilka must choose <span class="tex-font-style-bf">exactly two</span> sheep and take them to the mountains. If the beauty levels of these two sheep are $x$ and $y$ (after they have been fed), then Kamilka's <span class="tex-font-style-it">pleasure</span> from the walk is equal to $\gcd(x, y)$, where $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$. </p><p>The task is to find the maximum possible pleasure that Kamilka can get from the walk.</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains one integer $t$ ($1 \le t \le 500$), the number of test cases. The description of the test cases follows. </p><p> The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$), the number of sheep Kamilka has. </p><p> The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n \ (1 \le a_i \le 10^9)$ ¡ª the beauty levels of the sheep.</p><p>It is guaranteed that all $a_i$ are distinct.  </p></div><div class="output-specification"><p>For each test case, output a single integer: the maximum possible pleasure that Kamilka can get from the walk.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains one integer $t$ ($1 \le t \le 500$), the number of test cases. The description of the test cases follows. </p><p> The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$), the number of sheep Kamilka has. </p><p> The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_1, a_2, \ldots, a_n \ (1 \le a_i \le 10^9)$ ¡ª the beauty levels of the sheep.</p><p>It is guaranteed that all $a_i$ are distinct.  </p>

## Output

<p>For each test case, output a single integer: the maximum possible pleasure that Kamilka can get from the walk.</p>





```input1|2,3,6,7
4
2
1 3
5
5 4 3 2 1
3
5 6 7
3
1 11 10
```




```output1
2
4
2
10
```



## Note

<p>In the first test case, $d=1$ works. In this case, the pleasure is $\gcd(1+1, \ 1+3)=\gcd(2, \ 4)=2$. It can be shown that a greater answer cannot be obtained. </p><p> In the second test case, let's take $d=3$. In this case, the pleasure is $\gcd(1+3, \ 5+3)=\gcd(4, \ 8)=4$. Thus, for this test case, the answer is $4$.</p>
