## Description

<div><p>Gellyfish hates math problems, but she has to finish her math homework:</p><p>Gellyfish is given an array of $n$ positive integers $a_1, a_2, \ldots, a_n$.</p><p>She needs to do the following two-step operation until all elements of $a$ are equal:</p><ol> <li> Select two indexes $i$, $j$ satisfying $1 \leq i, j \leq n$ and $i \neq j$. </li><li> Replace $a_i$ with $\gcd(a_i, a_j)$. </li></ol><p>Now, Gellyfish asks you for the minimum number of operations to achieve her goal.</p><p>It can be proven that Gellyfish can always achieve her goal.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5000$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 5000$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of operations to achieve her goal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 5000$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 5000$)&nbsp;！ the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 5000$)&nbsp;！ the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of operations to achieve her goal.</p>





```input1|2,3,6,7
3
3
12 20 30
6
1 9 1 9 8 1
3
6 14 15
```




```output1
4
3
3
```



## Note

<p>In the first test case, the following is a way that minimizes the number of operations: </p><ol> <li> Choose $i = 3$ and $j=2$ and replace $a_3$ with $\gcd(a_3,a_2) = \gcd(30, 20) = 10$, then $a$ becomes $[12, 20, 10]$. </li><li> Choose $i=1$ and $j=3$ and replace $a_1$ with $\gcd(a_1,a_3) = \gcd(12, 10) = 2$, then $a$ becomes $[2, 20, 10]$. </li><li> Choose $i=2$ and $j=1$ and replace $a_2$ with $\gcd(a_2,a_1) = \gcd(20, 2) = 2$, then $a$ becomes $[2, 2, 10]$. </li><li> Choose $i=3$ and $j=1$ and replace $a_3$ with $\gcd(a_3,a_1) = \gcd(10, 2) = 2$, then $a$ becomes $[2, 2, 2]$. </li></ol>
