## Description

<div><p>Tonio's hometown of Morioh will be visited by $n$ important guests and for them, $m$ tables in the restaurant are reserved.</p><p>Every important guest has their own food preferences, the guest $i$ wants only the dish of the type $a_i$. <span class="tex-font-style-bf">Every guest</span> should be seated at some table, and at table $i$, no more than $c_i$ guests can be seated.</p><p><span class="tex-font-style-bf">For each table</span>, Tonio should determine the type of dish $x_i$ that will be served at this table. Then, only those guests at the table $i$ will be satisfied whose favorite dish is $x_i$.</p><p>Tonio was horrified by the number of guests, so he asked for your help. Find the maximum number of satisfied guests that can be obtained by optimally choosing the type of meal for each table and assigning guests to tables.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^3$, $1 \le m \le 2 \cdot 10^3$) ！ the number of important guests at Tonio and the number of tables available.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le n$) ！ where $a_i$ is the type of meal preferred by the $i$-th guest.</p><p>The third line contains $m$ integers $c_1$, $c_2$, ..., $c_m$ ($1 \le c_i \le 2 \cdot 10^3$), where $c_i$ is the $i$-th table capacity. It is guaranteed that $\sum_{i=1}^{m} c_i \geq n$. That is, there is enough space for all guests.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^3$, and the sum of $m$ over all test cases does not exceed $2 \cdot 10^3$.</p></div><div class="output-specification"><p>For each test case, print the maximum number of satisfied guests.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$).</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^3$, $1 \le m \le 2 \cdot 10^3$) ！ the number of important guests at Tonio and the number of tables available.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le n$) ！ where $a_i$ is the type of meal preferred by the $i$-th guest.</p><p>The third line contains $m$ integers $c_1$, $c_2$, ..., $c_m$ ($1 \le c_i \le 2 \cdot 10^3$), where $c_i$ is the $i$-th table capacity. It is guaranteed that $\sum_{i=1}^{m} c_i \geq n$. That is, there is enough space for all guests.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^3$, and the sum of $m$ over all test cases does not exceed $2 \cdot 10^3$.</p>

## Output

<p>For each test case, print the maximum number of satisfied guests.</p>





```input1|2,3,4,8,9,10,14,15,16
6
3 1
1 3 2
3
3 2
1 2 2
6 1
4 2
1 2 1 2
3 1
6 3
1 1 1 1 2 2
2 2 2
5 3
1 2 3 2 1
1 3 1
7 3
2 3 3 2 1 3 2
3 2 2
```




```output1
1
3
3
6
4
6
```



## Note

<p>In the first test case, there are $3$ guests and $1$ table, so only one guest will be satisfied in any case.</p><p>In the second test case, you can seat guests $2$ and $3$ at table $1$, and serve their favorite dish there, and seat the guest $1$ at table $2$, and serve the type $1$ dish. Thus, all guests will be satisfied. </p><p>In the third test case, it is optimal to seat guests $1$, $2$, and $3$ at table $1$, and to serve there the type $1$ dish, and to seat the guest $4$ at the second table and serve there the type $2$ dish. Then, only the guest number $3$ will be dissatisfied. </p>
