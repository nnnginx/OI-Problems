## Description

<div><p>Phoenix wonders what it is like to rob diamonds from a jewelry store!</p><p>There are $n$ types of diamonds. The $i$-th type has weight $w_i$ and value $v_i$. The store initially has $a_i$ diamonds of the $i$-th type.</p><p>Each day, for $q$ days, one of the following will happen: </p><ol> <li> A new shipment of $k_i$ diamonds of type $d_i$ arrive. </li><li> The store sells $k_i$ diamonds of type $d_i$. </li><li> Phoenix wonders what will happen if he robs the store using a bag that can fit diamonds with total weight not exceeding $c_i$. If he greedily takes diamonds of the largest value that fit, how much value would be taken? If there are multiple diamonds with the largest value, he will take the one with minimum weight. If, of the diamonds with the largest value, there are multiple with the same minimum weight, he will take any of them. </li></ol><p>Of course, since Phoenix is a law-abiding citizen, this is all a thought experiment and he never actually robs any diamonds from the store. This means that queries of type $3$ do not affect the diamonds in the store.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le q \le 10^5$)&nbsp;！ the number of types of diamonds and number of days, respectively.</p><p>The next $n$ lines describe each type of diamond. The $i$-th line will contain three integers $a_i$, $w_i$, and $v_i$ ($0 \le a_i \le 10^5$; $1 \le w_i, v_i \le 10^5$)&nbsp;！ the initial number of diamonds of the $i$-th type, the weight of diamonds of the $i$-th type, and the value of diamonds of the $i$-th type, respectively.</p><p>The next $q$ lines contain the queries. For each query, the first integer of each line is $t$ ($1 \le t \le 3$)&nbsp;！ the type of query.</p><p>If $t=1$, then two integers $k_i$, $d_i$ follow ($1 \le k_i \le 10^5$; $1 \le d_i \le n$). This means that a new shipment of $k_i$ diamonds arrived, each of type $d_i$.</p><p>If $t=2$, then two integers $k_i$, $d_i$ follow ($1 \le k_i \le 10^5$; $1 \le d_i \le n$). This means that the store has sold $k_i$ diamonds, each of type $d_i$. It is guaranteed that the store had the diamonds before they sold them.</p><p>If $t=3$, an integer $c_i$ will follow ($1 \le c_i \le 10^{18}$)&nbsp;！ the weight capacity of Phoenix's bag.</p><p>It is guaranteed that there is at least one query where $t=3$.</p></div><div class="output-specification"><p>Print the answer for each query of the third type ($t=3$).</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 2 \cdot 10^5$; $1 \le q \le 10^5$)&nbsp;！ the number of types of diamonds and number of days, respectively.</p><p>The next $n$ lines describe each type of diamond. The $i$-th line will contain three integers $a_i$, $w_i$, and $v_i$ ($0 \le a_i \le 10^5$; $1 \le w_i, v_i \le 10^5$)&nbsp;！ the initial number of diamonds of the $i$-th type, the weight of diamonds of the $i$-th type, and the value of diamonds of the $i$-th type, respectively.</p><p>The next $q$ lines contain the queries. For each query, the first integer of each line is $t$ ($1 \le t \le 3$)&nbsp;！ the type of query.</p><p>If $t=1$, then two integers $k_i$, $d_i$ follow ($1 \le k_i \le 10^5$; $1 \le d_i \le n$). This means that a new shipment of $k_i$ diamonds arrived, each of type $d_i$.</p><p>If $t=2$, then two integers $k_i$, $d_i$ follow ($1 \le k_i \le 10^5$; $1 \le d_i \le n$). This means that the store has sold $k_i$ diamonds, each of type $d_i$. It is guaranteed that the store had the diamonds before they sold them.</p><p>If $t=3$, an integer $c_i$ will follow ($1 \le c_i \le 10^{18}$)&nbsp;！ the weight capacity of Phoenix's bag.</p><p>It is guaranteed that there is at least one query where $t=3$.</p>

## Output

<p>Print the answer for each query of the third type ($t=3$).</p>

## Samples

```input1
3 5
2 3 4
1 5 1
0 2 4
3 6
1 3 3
3 10
2 2 3
3 30
```

```output1
8
16
13
```




## Note

<p>For the first query where $t=3$, Phoenix can fit $2$ diamonds of type $1$, with total weight $6$ and value $8$.</p><p>For the second query where $t=3$, Phoenix will first fit in $3$ diamonds of type $3$, then one diamond of type $1$ for a total weight of $9$ and a value of $16$. Note that diamonds of type $3$ are prioritized over type $1$ because type $3$ has equal value but less weight.</p><p>For the final query where $t=3$, Phoenix can fit every diamond for a total value of $13$.</p>
