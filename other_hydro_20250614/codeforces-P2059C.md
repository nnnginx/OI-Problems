## Description

<div><p>Nikyr has started working as a queue manager at the company "Black Contour." He needs to choose the order of servicing customers. There are a total of $n$ queues, each initially containing $0$ people. In each of the next $n$ moments of time, there are <span class="tex-font-style-bf">two sequential</span> events:</p><ol><li> New customers arrive in all queues. More formally, at the $j$-th moment of time, the number of people in the $i$-th queue increases by a <span class="tex-font-style-bf">positive</span> integer $a_{i,j}$.</li><li> Nikyr chooses <span class="tex-font-style-bf">exactly one</span> of the $n$ queues to be served at that moment in time. The number of customers in this queue becomes $0$.</li></ol><p>Let the number of people in the $i$-th queue after all events be $x_i$. Nikyr wants MEX$^{\dagger}$ of the collection $x_1, x_2, \ldots, x_n$ to be as large as possible. Help him determine the maximum value he can achieve with an optimal order of servicing the queues.</p><p>$^{\dagger}$The minimum excluded (MEX) of a collection of integers $c_1, c_2, \ldots, c_k$ is defined as the smallest non-negative integer $y$ which does not occur in the collection $c$. </p><p>For example: </p><ul> <li> $\operatorname{MEX}([2,2,1])= 0$, since $0$ does not belong to the array. </li><li> $\operatorname{MEX}([3,1,0,1]) = 2$, since $0$ and $1$ belong to the array, but $2$ does not. </li><li> $\operatorname{MEX}([0,3,1,2]) = 4$, since $0$, $1$, $2$, and $3$ belong to the array, but $4$ does not. </li></ul></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 300$) �� the number of queues and moments of time.</p><p>The $i$-th of the next $n$ lines contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($1 \le a_{i,j} \le 10^9$) �� the number of new customers in the $i$-th queue at each moment of time.</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer �� the maximum value of $\operatorname{MEX}([x_1, x_2, \ldots, x_n])$ that can be achieved.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) �� the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 300$) �� the number of queues and moments of time.</p><p>The $i$-th of the next $n$ lines contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($1 \le a_{i,j} \le 10^9$) �� the number of new customers in the $i$-th queue at each moment of time.</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer �� the maximum value of $\operatorname{MEX}([x_1, x_2, \ldots, x_n])$ that can be achieved.</p>





```input1|2,3,4,8,9,10,11
4
2
1 2
2 1
2
10 10
10 10
3
2 3 3
4 4 1
2 1 1
4
4 2 2 17
1 9 3 1
5 5 5 11
1 2 1 1
```




```output1
2
1
3
3
```



## Note

<p>In the first test case, the second queue can be served at time $1$, and the first queue at time $2$. There will be $x_1 = 0$ people left in the first queue and $x_2 = 1$ person left in the second queue. Therefore, the answer is $\operatorname{MEX}([0, 1]) = 2$.</p><p>In the second test case, the first queue can be served both times. There will be $x_1 = 0$ people left in the first queue and $x_2 = 20$ people left in the second queue. Therefore, the answer is $\operatorname{MEX}([0, 20]) = 1$.</p><p>In the third test case, the third queue can be served at time $1$, the second queue at time $2$, and the first queue at time $3$. There will be $x_1 = 0$ people left in the first queue, $x_2 = 1$ person left in the second queue, and $x_3 = 2$ people left in the third queue. Therefore, the answer is $\operatorname{MEX}([0, 1, 2]) = 3$.</p>
