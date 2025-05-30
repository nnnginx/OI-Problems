## Description

<div><p><span class="tex-font-style-it">Lunar New Year is approaching, and Bob is planning to go for a famous restaurant �� "Alice's".</span></p><p>The restaurant "Alice's" serves $n$ kinds of food. The cost for the $i$-th kind is always $c_i$. Initially, the restaurant has enough ingredients for serving exactly $a_i$ dishes of the $i$-th kind. In the New Year's Eve, $m$ customers will visit Alice's one after another and the $j$-th customer will order $d_j$ dishes of the $t_j$-th kind of food. The $(i + 1)$-st customer will only come after the $i$-th customer is completely served.</p><p>Suppose there are $r_i$ dishes of the $i$-th kind remaining (initially $r_i = a_i$). When a customer orders $1$ dish of the $i$-th kind, the following principles will be processed.</p><ol><li> If $r_i &gt; 0$, the customer will be served exactly $1$ dish of the $i$-th kind. The cost for the dish is $c_i$. Meanwhile, $r_i$ will be reduced by $1$.</li><li> Otherwise, the customer will be served $1$ dish of the <span class="tex-font-style-bf">cheapest</span> available kind of food if there are any. If there are multiple cheapest kinds of food, the one with the smallest index among the cheapest will be served. The cost will be the cost for the dish served and the remain for the corresponding dish will be reduced by $1$.</li><li> If there are no more dishes at all, the customer will leave angrily. Therefore, no matter how many dishes are served previously, the cost for the customer is $0$.</li></ol><p>If the customer doesn't leave after the $d_j$ dishes are served, the cost for the customer will be the sum of the cost for these $d_j$ dishes.</p><p>Please determine the total cost for each of the $m$ customers.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^5$), representing the number of different kinds of food and the number of customers, respectively.</p><p>The second line contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$), where $a_i$ denotes the initial remain of the $i$-th kind of dishes.</p><p>The third line contains $n$ positive integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 10^6$), where $c_i$ denotes the cost of one dish of the $i$-th kind.</p><p>The following $m$ lines describe the orders of the $m$ customers respectively. The $j$-th line contains two positive integers $t_j$ and $d_j$ ($1 \leq t_j \leq n$, $1 \leq d_j \leq 10^7$), representing the kind of food and the number of dishes the $j$-th customer orders, respectively.</p></div><div class="output-specification"><p>Print $m$ lines. In the $j$-th line print the cost for the $j$-th customer.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n, m \leq 10^5$), representing the number of different kinds of food and the number of customers, respectively.</p><p>The second line contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$), where $a_i$ denotes the initial remain of the $i$-th kind of dishes.</p><p>The third line contains $n$ positive integers $c_1, c_2, \ldots, c_n$ ($1 \leq c_i \leq 10^6$), where $c_i$ denotes the cost of one dish of the $i$-th kind.</p><p>The following $m$ lines describe the orders of the $m$ customers respectively. The $j$-th line contains two positive integers $t_j$ and $d_j$ ($1 \leq t_j \leq n$, $1 \leq d_j \leq 10^7$), representing the kind of food and the number of dishes the $j$-th customer orders, respectively.</p>

## Output

<p>Print $m$ lines. In the $j$-th line print the cost for the $j$-th customer.</p>

## Samples

```input1
8 5
8 6 2 1 4 5 7 5
6 3 3 2 6 2 3 2
2 8
1 4
4 7
3 4
6 10
```

```output1
22
24
14
10
39
```






```input2
6 6
6 6 6 6 6 6
6 66 666 6666 66666 666666
1 6
2 6
3 6
4 6
5 6
6 66
```

```output2
36
396
3996
39996
399996
0
```






```input3
6 6
6 6 6 6 6 6
6 66 666 6666 66666 666666
1 6
2 13
3 6
4 11
5 6
6 6
```

```output3
36
11058
99996
4333326
0
0
```




## Note

<p>In the first sample, $5$ customers will be served as follows.</p><ol><li> Customer $1$ will be served $6$ dishes of the $2$-nd kind, $1$ dish of the $4$-th kind, and $1$ dish of the $6$-th kind. The cost is $6 \cdot 3 + 1 \cdot 2 + 1 \cdot 2 = 22$. The remain of the $8$ kinds of food will be $\{8, 0, 2, 0, 4, 4, 7, 5\}$.</li><li> Customer $2$ will be served $4$ dishes of the $1$-st kind. The cost is $4 \cdot 6 = 24$. The remain will be $\{4, 0, 2, 0, 4, 4, 7, 5\}$.</li><li> Customer $3$ will be served $4$ dishes of the $6$-th kind, $3$ dishes of the $8$-th kind. The cost is $4 \cdot 2 + 3 \cdot 2 = 14$. The remain will be $\{4, 0, 2, 0, 4, 0, 7, 2\}$.</li><li> Customer $4$ will be served $2$ dishes of the $3$-rd kind, $2$ dishes of the $8$-th kind. The cost is $2 \cdot 3 + 2 \cdot 2 = 10$. The remain will be $\{4, 0, 0, 0, 4, 0, 7, 0\}$.</li><li> Customer $5$ will be served $7$ dishes of the $7$-th kind, $3$ dishes of the $1$-st kind. The cost is $7 \cdot 3 + 3 \cdot 6 = 39$. The remain will be $\{1, 0, 0, 0, 4, 0, 0, 0\}$.</li></ol><p>In the second sample, each customer is served what they order <span class="tex-font-style-bf">except</span> the last one, who leaves angrily without paying. For example, the second customer is served $6$ dishes of the second kind, so the cost is $66 \cdot 6 = 396$.</p><p>In the third sample, some customers may not be served what they order. For example, the second customer is served $6$ dishes of the second kind, $6$ of the third and $1$ of the fourth, so the cost is $66 \cdot 6 + 666 \cdot 6 + 6666 \cdot 1 = 11058$.</p>
