## Description

<div><p>One day, the schoolboy Mark misbehaved, so the teacher Sasha called him to the whiteboard.</p><p>Sasha gave Mark a table with $n$ rows and $m$ columns. His task is to arrange the numbers $0, 1, \ldots, n \cdot m - 1$ in the table (each number must be used exactly once) in such a way as to maximize the sum of MEX$^{\text{∗}}$ across all rows and columns. More formally, he needs to maximize $$\sum\limits_{i = 1}^{n} \operatorname{mex}(\{a_{i,1}, a_{i,2}, \ldots, a_{i,m}\}) + \sum\limits_{j = 1}^{m} \operatorname{mex}(\{a_{1,j}, a_{2,j}, \ldots, a_{n,j}\}),$$ where $a_{i,j}$ is the number in the $i$-th row and $j$-th column.</p><p>Sasha is not interested in how Mark arranges the numbers, so he only asks him to state one number&nbsp;— the maximum sum of MEX across all rows and columns that can be achieved.</p><div class="statement-footnote"><p>$^{\text{∗}}$The minimum excluded (MEX) of a collection of integers $c_1, c_2, \ldots, c_k$ is defined as the smallest non-negative integer $x$ which does not occur in the collection $c$. </p><p>For example: </p><ul> <li> $\operatorname{mex}([2,2,1])= 0$, since $0$ does not belong to the array. </li><li> $\operatorname{mex}([3,1,0,1]) = 2$, since $0$ and $1$ belong to the array, but $2$ does not. </li><li> $\operatorname{mex}([0,3,1,2]) = 4$, since $0$, $1$, $2$, and $3$ belong to the array, but $4$ does not. </li></ul></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^9$)&nbsp;— the number of rows and columns in the table, respectively.</p></div><div class="output-specification"><p>For each test case, output the maximum possible sum of $\operatorname{mex}$ across all rows and columns.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 10^9$)&nbsp;— the number of rows and columns in the table, respectively.</p>

## Output

<p>For each test case, output the maximum possible sum of $\operatorname{mex}$ across all rows and columns.</p>





```input1|2,4
3
1 1
2 2
3 5
```




```output1
2
3
6
```



## Note

<p>In the first test case, the only element is $0$, and the sum of the $\operatorname{mex}$ of the numbers in the first row and the $\operatorname{mex}$ of the numbers in the first column is $\operatorname{mex}(\{0\}) + \operatorname{mex}(\{0\}) = 1 + 1 = 2$.</p><p>In the second test case, the optimal table may look as follows:</p><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr></tbody></table><p></p><p>Then $\sum\limits_{i = 1}^{n} \operatorname{mex}(\{a_{i,1}, a_{i,2}, \ldots, a_{i,m}\}) + \sum\limits_{j = 1}^{m} \operatorname{mex}(\{a_{1,j}, a_{2,j}, \ldots, a_{n,j}\}) = \operatorname{mex}(\{3, 0\}) + \operatorname{mex}(\{2, 1\})$ $+ \operatorname{mex}(\{3, 2\}) + \operatorname{mex}(\{0, 1\}) = 1 + 0 + 0 + 2 = 3$.</p>
