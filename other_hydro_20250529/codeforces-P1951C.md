## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/6TpyRE_juyA"><span class="tex-font-style-it">Maître Gims - Est-ce que tu m'aimes ?</span></a></div><div class="epigraph-source">ඞ</div></div><p>As the CEO of a startup company, you want to reward each of your $k$ employees with a ticket to the upcoming concert. The tickets will be on sale for $n$ days, and by some time travelling, you have predicted that the price per ticket at day $i$ will be $a_i$. However, to prevent ticket hoarding, the concert organizers have implemented the following measures:</p><ul> <li> A person may purchase no more than $m$ tickets per day. </li><li> If a person purchases $x$ tickets on day $i$, all subsequent days (i.e. from day $i+1$ onwards) will have their prices per ticket increased by $x$. </li></ul><p>For example, if $a = [1, 3, 8, 4, 5]$ and you purchase $2$ tickets on day $1$, they will cost $2$ in total, and the prices from day $2$ onwards will become $[5, 10, 6, 7]$. If you then purchase $3$ more tickets on day $2$, they will cost in total an additional $15$, and the prices from day $3$ onwards will become $[13, 9, 10]$.</p><p>Find the minimum spending to purchase $k$ tickets.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n \le 3 \cdot 10^5, 1 \le m \le 10^9, 1 \le k \le \min(nm, 10^9)$)&nbsp;— the number of sale days, the maximum amount of ticket purchasable each day, and the number of tickets to be bought at the end.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the price per ticket for each of the upcoming $n$ days.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer: the minimum amount of money needed to purchase exactly $k$ tickets.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($1 \le n \le 3 \cdot 10^5, 1 \le m \le 10^9, 1 \le k \le \min(nm, 10^9)$)&nbsp;— the number of sale days, the maximum amount of ticket purchasable each day, and the number of tickets to be bought at the end.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the price per ticket for each of the upcoming $n$ days.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer: the minimum amount of money needed to purchase exactly $k$ tickets.</p>





```input1|2,3,6,7
4
4 2 3
8 6 4 2
4 2 8
8 6 4 2
5 100 1
10000 1 100 10 1000
6 3 9
5 5 5 5 5 5
```




```output1
10
64
1
72
```



## Note

<p>In the first test case, one optimal way to buy $3$ tickets is as follows: </p><ul> <li> Buy $0$ tickets on the first day. The prices per ticket for the remaining days are $[6, 4, 2]$. </li><li> Buy $0$ tickets on the second day. The prices per ticket for the remaining days are $[4, 2]$. </li><li> Buy $1$ ticket on the third day with cost $4$. The price per ticket for the remaining day is $[3]$. </li><li> Buy $2$ tickets on the fourth day with cost $6$. </li></ul><p>In the second test case, there is only one way to buy $8$ tickets: </p><ul> <li> Buy $2$ tickets on the first day with cost $16$. The prices per ticket for the remaining days are $[8, 6, 4]$. </li><li> Buy $2$ tickets on the second day with cost $16$. The prices per ticket for the remaining days are $[8, 6]$. </li><li> Buy $2$ tickets on the third day with cost $16$. The price per ticket for the remaining day is $[8]$. </li><li> Buy $2$ tickets on the fourth day with cost $16$. </li></ul>
