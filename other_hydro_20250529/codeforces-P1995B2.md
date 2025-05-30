## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that in this version, instead of listing the number of petals for each flower, the number of petals and the quantity of flowers in the store is set for all types of flowers.</span></p><p>A girl is preparing for her birthday and wants to buy the most beautiful bouquet. There are a total of $n$ different types of flowers in the store, each of which is characterized by the number of petals and the quantity of this type of flower. A flower with $k$ petals costs $k$ coins. The girl has decided that the difference in the number of petals between any two flowers she will use to decorate her cake should not exceed one. At the same time, the girl wants to assemble a bouquet with the maximum possible number of petals. Unfortunately, she only has $m$ coins, and she cannot spend more. What is the maximum total number of petals she can assemble in the bouquet?</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. This is followed by descriptions of the test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \le n \le 2 \cdot 10^5, 1 \le m \le 10^{18}$)&nbsp;！ the number of types of flowers in the store and the number of coins the girl possesses, respectively. The second line of each test case contains $n$ <span class="tex-font-style-bf">different</span> integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of petals of the $i$-th flower type in the store (for different indexes $i \neq j$, it must be $a_i \neq a_j$). The third line of each test case contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 10^9$), where $c_i$ is the quantity of the $i$-th flower type in the store.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot {10}^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;！ the maximum possible number of petals in a bouquet that a girl can collect, observing all the conditions listed above.</p></div>

## Input

<p>Each test consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10\,000$)&nbsp;！ the number of test cases. This is followed by descriptions of the test cases.</p><p>The first line of each test case contains two integers $n$, $m$ ($1 \le n \le 2 \cdot 10^5, 1 \le m \le 10^{18}$)&nbsp;！ the number of types of flowers in the store and the number of coins the girl possesses, respectively. The second line of each test case contains $n$ <span class="tex-font-style-bf">different</span> integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of petals of the $i$-th flower type in the store (for different indexes $i \neq j$, it must be $a_i \neq a_j$). The third line of each test case contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 10^9$), where $c_i$ is the quantity of the $i$-th flower type in the store.</p><p>The sum of $n$ over all test cases does not exceed $2 \cdot {10}^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;！ the maximum possible number of petals in a bouquet that a girl can collect, observing all the conditions listed above.</p>





```input1|2,3,4,8,9,10,14,15,16,20,21,22
7
3 10
1 2 3
2 2 1
3 1033
206 207 1000
3 4 1
6 20
4 2 7 5 6 1
1 2 1 3 1 7
8 100000
239 30 610 122 24 40 8 2
12 13123 112 1456 124 100 123 10982
6 13
2 4 11 1 3 5
2 2 1 2 2 1
8 10330
206 210 200 201 198 199 222 1000
9 10 11 12 13 14 15 16
2 10000000000
11 12
87312315 753297050
```




```output1
7
1033
19
99990
13
10000
9999999999
```



## Note

<p>In the first test case, some valid bouquets are $(1, 1, 2, 2), (2, 2, 3), (1, 1), (2, 2)$. The maximum over all valid bouquets not greater than $10$ is $7$ for $(2, 2, 3)$. In the second test case, you can assemble a valid bouquet with $(206, 206, 207, 207, 207)$ with a sum of $1033$, which is the maximum number of petals the girl can buy. In the third test case, you can assemble a valid bouquet with $(5, 5, 5, 4)$ with a sum of $19$. It can be seen that no valid bouquet can have $20$ petals.</p>
