## Description

<div><p>One day, the teachers of "T-generation" decided to instill discipline in the pupils, so they lined them up and made them calculate in order. There are a total of $n$ pupils, the height of the $i$-th pupil in line is $a_i$. </p><p>The line is <span class="tex-font-style-it">comfortable</span>, if for each $i$ from $1$ to $n - 1$, the following condition holds: $a_i \cdot 2 \ge a_{i + 1}$. Initially, the line is comfortable.</p><p>The teachers do not like that the maximum height in the line is too small, so they want to feed the pupils pizza. You know that when a pupil eats one pizza, their height increases by $1$. One pizza can only be eaten by only one pupil, but each pupil can eat an unlimited number of pizzas. It is important that after all the pupils have eaten their pizzas, the line is comfortable.</p><p>The teachers have $q$ options for how many pizzas they will order. For each option $k_i$, answer the question: what is the maximum height $\max(a_1, a_2, \ldots, a_n)$ that can be achieved if the pupils eat at most $k_i$ pizzas.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line of each set of test case contains two integers $n$ and $q$ ($1 \le n, q \le 5 \cdot 10^4$)&nbsp;�� the number of pupils and the number of options for how many pizzas the teachers will order.</p><p>The second line of each set of test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;�� the heights of the pupils.It is guaranteed that initially, the line is comfortable.</p><p>Each of the following $q$ lines of each set of input data contains one integer $k_i$ ($1 \le k_i \le 10^9$)&nbsp;�� the next limit for how many pizzas the pupils can eat.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of input data does not exceed $5 \cdot 10^4$.</p><p>It is guaranteed that the sum of the values of $q$ across all sets of input data does not exceed $5 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, for each limit for how many pizzas the pupils can eat, output the maximum value $\max(a_1, a_2, \ldots, a_n)$ that can be achieved while ensuring that the line is comfortable.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;�� the number of test cases. The description of the test cases follows.</p><p>The first line of each set of test case contains two integers $n$ and $q$ ($1 \le n, q \le 5 \cdot 10^4$)&nbsp;�� the number of pupils and the number of options for how many pizzas the teachers will order.</p><p>The second line of each set of test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;�� the heights of the pupils.It is guaranteed that initially, the line is comfortable.</p><p>Each of the following $q$ lines of each set of input data contains one integer $k_i$ ($1 \le k_i \le 10^9$)&nbsp;�� the next limit for how many pizzas the pupils can eat.</p><p>It is guaranteed that the sum of the values of $n$ across all sets of input data does not exceed $5 \cdot 10^4$.</p><p>It is guaranteed that the sum of the values of $q$ across all sets of input data does not exceed $5 \cdot 10^4$.</p>

## Output

<p>For each test case, for each limit for how many pizzas the pupils can eat, output the maximum value $\max(a_1, a_2, \ldots, a_n)$ that can be achieved while ensuring that the line is comfortable.</p>





```input1|2,3,4,14,15,16,17,18,19
3
2 1
10 20
10
6 7
3 1 2 4 5 6
1
2
4
8
16
32
64
10 4
1 2 4 8 16 32 64 128 256 512
10
100
1000
10000
```




```output1
26
7 8 10 12 19 35 67
513 560 1011 10001
```



## Note

<p>In the first query of the first set of input data, you can first give $3$ pizzas to the first pupil, and then give $6$ pizzas to the second pupil, making the final array $[13, 26]$ (the line is comfortable since $13 \cdot 2 \ge 26$), and the maximum element in it is $26$.</p>
