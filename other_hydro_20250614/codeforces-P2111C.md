## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$, consisting of $n$ integers.</p><p>In one operation, you are allowed to perform one of the following actions: </p><ul> <li> Choose a position $i$ ($1 &lt; i \le n$) and make all elements to the left of $i$ equal to $a_i$. That is, assign the value $a_i$ to all $a_j$ ($1 \le j &lt; i$). The cost of such an operation is $(i - 1) \cdot a_i$. </li><li> Choose a position $i$ ($1 \le i &lt; n$) and make all elements to the right of $i$ equal to $a_i$. That is, assign the value $a_i$ to all $a_j$ ($i &lt; j \le n$). The cost of such an operation is $(n - i) \cdot a_i$. </li></ul><p>Note that the elements affected by an operation may already be equal to $a_i$, but that doesn't change the cost.</p><p>You are allowed to perform any number of operations (including zero). What is the minimum total cost to make all elements of the array equal?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the minimum total cost of operations to make all elements of the array equal.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the minimum total cost of operations to make all elements of the array equal.</p>





```input1|2,3,6,7
3
4
2 4 1 3
3
1 1 1
10
7 5 5 5 10 9 9 4 6 10
```




```output1
3
0
35
```



## Note

<p>In the first test case, you can perform the operation twice: </p><ul> <li> choose $i = 3$ and make all elements to the left of it equal to it, the cost will be $2 \cdot 1 = 2$; </li><li> choose $i = 3$ and make all elements to the right of it equal to it, the cost will be $1 \cdot 1 = 1$. </li></ul><p>The total cost is $2 + 1 = 3$.</p><p>In the second test case, all elements are already equal, so no operations need to be performed.</p>
