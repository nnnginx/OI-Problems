## Description

<div><p>Timur is in a car traveling on the number line from point $0$ to point $n$. The car starts moving from point $0$ at minute $0$.</p><p>There are $k+1$ signs on the line at points $0, a_1, a_2, \dots, a_k$, and Timur knows that the car will arrive there at minutes $0, b_1, b_2, \dots, b_k$, respectively. The sequences $a$ and $b$ are strictly increasing with $a_k = n$.</p><center> <img class="tex-graphics" src="./34656/file/aYAETYy3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Between any two adjacent signs, the car travels with a <span class="tex-font-style-bf">constant speed</span>. Timur has $q$ queries: each query will be an integer $d$, and Timur wants you to output how many minutes it takes the car to reach point $d$, <span class="tex-font-style-bf">rounded down to the nearest integer</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$, ($k \leq n \leq 10^9$; $1 \leq k, q \leq 10^5$)&nbsp;！ the final destination, the number of points Timur knows the time for, and the number of queries respectively.</p><p>The second line of each test case contains $k$ integers $a_i$ ($1 \leq a_i \leq n$; $a_i &lt; a_{i+1}$ for every $1 \leq i \leq k-1$; $a_k = n$). </p><p>The third line of each test case contains $k$ integers $b_i$ ($1 \leq b_i \leq 10^9$; $b_i &lt; b_{i+1}$ for every $1 \leq i \leq k-1$).</p><p>Each of the following $q$ lines contains a single integer $d$ ($0 \leq d \leq n$)&nbsp;！ the distance that Timur asks the minutes passed for.</p><p>The sum of $k$ over all test cases doesn't exceed $10^5$, and the sum of $q$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each query, output a single integer&nbsp;！ the number of minutes passed until the car reaches the point $d$, rounded down.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $k$, and $q$, ($k \leq n \leq 10^9$; $1 \leq k, q \leq 10^5$)&nbsp;！ the final destination, the number of points Timur knows the time for, and the number of queries respectively.</p><p>The second line of each test case contains $k$ integers $a_i$ ($1 \leq a_i \leq n$; $a_i &lt; a_{i+1}$ for every $1 \leq i \leq k-1$; $a_k = n$). </p><p>The third line of each test case contains $k$ integers $b_i$ ($1 \leq b_i \leq 10^9$; $b_i &lt; b_{i+1}$ for every $1 \leq i \leq k-1$).</p><p>Each of the following $q$ lines contains a single integer $d$ ($0 \leq d \leq n$)&nbsp;！ the distance that Timur asks the minutes passed for.</p><p>The sum of $k$ over all test cases doesn't exceed $10^5$, and the sum of $q$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each query, output a single integer&nbsp;！ the number of minutes passed until the car reaches the point $d$, rounded down.</p>





```input1|2,3,4,5,6,7,15,16,17,18
4
10 1 3
10
10
0
6
7
10 2 4
4 10
4 7
6
4
2
7
1000000000 1 1
1000000000
1000000000
99999999
6 1 3
6
5
2
6
5
```




```output1
0 6 7 
5 4 2 5 
99999999 
1 5 4
```



## Note

<p>For the first test case, the car goes from point $0$ to point $10$ in $10$ minutes, so the speed is $1$ unit per minute and:</p><ul> <li> At point $0$, the time will be $0$ minutes. </li><li> At point $6$, the time will be $6$ minutes. </li><li> At point $7$, the time will be $7$ minutes. </li></ul><p>For the second test case, between points $0$ and $4$, the car travels at a speed of $1$ unit per minute and between $4$ and $10$ with a speed of $2$ units per minute and:</p><ul> <li> At point $6$, the time will be $5$ minutes. </li><li> At point $4$, the time will be $4$ minutes. </li><li> At point $2$, the time will be $2$ minutes. </li><li> At point $7$, the time will be $5.5$ minutes, so the answer is $5$. </li></ul><p>For the fourth test case, the car travels with $1.2$ units per minute, so the answers to the queries are:</p><ul> <li> At point $2$, the time will be $1.66\dots$ minutes, so the answer is $1$. </li><li> At point $6$, the time will be $5$ minutes. </li><li> At point $5$, the time will be $4.16\dots$ minutes, so the answer is $4$. </li></ul>
