## Description

<div><p>Piggy Zhou loves matrices, especially those that make him get excited, called <span class="tex-font-style-it">hot matrix</span>.</p><p>A hot matrix of size $n \times n$ can be defined as follows. Let $a_{i, j}$ denote the element in the $i$-th row, $j$-th column ($1 \le i, j \le n$).</p><ol><li> Each column and row of the matrix is a permutation of all numbers from $0$ to $n-1$. </li><li> For each pair of indices $i$, $j$, such that $1 \le i, j \le n$, $a_{i, j} + a_{i, n - j + 1} = n - 1$. </li><li> For each pair of indices $i$, $j$, such that $1 \le i, j \le n$, $a_{i, j} + a_{n - i + 1, j} = n - 1$. </li><li> All ordered pairs $\left(a_{i, j}, a_{i, j + 1}\right)$, where $1 \le i \le n$, $1 \le j &lt; n$, are distinct. </li><li> All ordered pairs $\left(a_{i, j}, a_{i + 1, j}\right)$, where $1 \le i &lt; n$, $1 \le j \le n$, are distinct.</li></ol><p>Now, Piggy Zhou gives you a number $n$, and you need to provide him with a hot matrix if the hot matrix exists for the given $n$, or inform him that he will never get excited if the hot matrix does not exist for the given $n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The only line of each test case contains one integer $n$ ($1 \le n \le 3000$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $3000$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">NO</span>" (without quotes) if the hot matrix does not exist for the given $n$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line. Then output $n$ rows, with $n$ numbers in each row, representing the hot matrix of size $n\times n$ that meets the requirements of the problem.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The only line of each test case contains one integer $n$ ($1 \le n \le 3000$).</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $3000$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">NO</span>" (without quotes) if the hot matrix does not exist for the given $n$.</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line. Then output $n$ rows, with $n$ numbers in each row, representing the hot matrix of size $n\times n$ that meets the requirements of the problem.</p><p>If there are multiple solutions, print any of them.</p>





```input1|2,4
4
1
2
3
4
```




```output1
YES
0
YES
0 1
1 0
NO
YES
0 1 2 3
1 3 0 2
2 0 3 1
3 2 1 0
```



## Note

<p>In the first, second and fourth test case, it can be verified that the matrix provided in the example meets all the conditions stated in the problem.</p><p>In the third test case, by enumerating all possible matrices, it can be proven that there is no hot matrix that satisfies the conditions of the problem.</p>
