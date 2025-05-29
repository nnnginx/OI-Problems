## Description

<div><p>For her birthday, each of Asuna's $n$ admirers gifted her a tower. The height of the tower from the $i$-th admirer is equal to $a_i$. </p><p>Asuna evaluates the beauty of the received gifts as $\max(a_1, a_2, \ldots, a_n)$. She can perform the following operation an arbitrary number of times (possibly, zero). </p><ul> <li> Take such $1 \le i \neq j \le n$ that $a_i + a_j$ is odd and $a_i &gt; 0$, then decrease $a_i$ by $1$ and increase $a_j$ by $1$. </li></ul> It is easy to see that the heights of the towers remain non-negative during the operations. <p>Help Asuna find the maximum possible beauty of the gifts after any number of operations!</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) ！ the number of admirers of Asuna.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n \ (1 \le a_i \le 10^9)$ ！ the heights of the towers.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer: the maximum value of the beauty of the gifts that Asuna can achieve.</p></div>

## Input

<p>Each test consists of several test cases. The first line of the input data contains one integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) ！ the number of admirers of Asuna.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n \ (1 \le a_i \le 10^9)$ ！ the heights of the towers.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer: the maximum value of the beauty of the gifts that Asuna can achieve.</p>





```input1|2,3,6,7
4
3
5 3 9
2
3 2
4
1 2 2 1
5
5 4 3 2 9
```




```output1
9
5
5
21
```



## Note

<p>In the first test case, no pair of towers satisfies the required condition for applying the operation, so no operations can be performed. In this case, the answer is $\max(5, \ 3, \ 9) = 9$.</p><p>In the second test case, the operation with $i = 2$ and $j = 1$ can be applied twice. After that, the array becomes: $a \ = \ [5, \ 0]$. Thus, the answer is 5.</p><p>In the third test case, the following sequence of operations can be applied:</p><ol><li> Operation with $i=1$ and $j=2$.<p>$[1, \ 2, \ 2, \ 1] \quad \rightarrow \quad [0, \ 3, \ 2, \ 1]$</p></li><li> Operation with $i=3$ and $j=2$.<p>$[0, \ 3, \ 2, \ 1] \quad \rightarrow \quad [0, \ 4, \ 1, \ 1]$</p></li><li> Operation with $i=3$ and $j=2$.<p>$[0, \ 4, \ 1, \ 1] \quad \rightarrow \quad [0, \ 5, \ 0, \ 1]$</p></li></ol><p>$\max(0, \ 5, \ 0, \ 1) \ = \ 5$.</p><p>Therefore, the answer is 5.</p>
