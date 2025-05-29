## Description

<div><p>A <span class="tex-font-style-it">multiset</span> is a set of numbers in which there can be equal elements, and the order of the numbers does not matter. For example, $\{2,2,4\}$ is a multiset.</p><p>You have a multiset $S$. Initially, the multiset contains only one positive integer $n$. That is, $S=\{n\}$. Additionally, there is a given positive integer $k$.</p><p>In one operation, you can select any positive integer $u$ in $S$ and remove one copy of $u$ from $S$. Then, insert no more than $k$ positive integers into $S$ so that the sum of all inserted integers is equal to $u$.</p><p>Find the minimum number of operations to make $S$ contain $n$ ones.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line of each testcase contains two integers $n,k$ ($1\le n\le 1000,2\le k\le 1000$).</p></div><div class="output-specification"><p>For each testcase, print one integer, which is the required answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The only line of each testcase contains two integers $n,k$ ($1\le n\le 1000,2\le k\le 1000$).</p>

## Output

<p>For each testcase, print one integer, which is the required answer.</p>





```input1|2,4
4
1 5
5 2
6 3
16 4
```




```output1
0
4
3
5
```



## Note

<p>For the first test case, initially $S=\{1\}$, already satisfying the requirement. Therefore, we need zero operations.</p><p>For the second test case, initially $S=\{5\}$. We can apply the following operations:</p><ul> <li> Select $u=5$, remove $u$ from $S$, and insert $2,3$ into $S$. Now, $S=\{2,3\}$. </li><li> Select $u=2$, remove $u$ from $S$, and insert $1,1$ into $S$. Now, $S=\{1,1,3\}$. </li><li> Select $u=3$, remove $u$ from $S$, and insert $1,2$ into $S$. Now, $S=\{1,1,1,2\}$. </li><li> Select $u=2$, remove $u$ from $S$, and insert $1,1$ into $S$. Now, $S=\{1,1,1,1,1\}$. </li></ul><p>Using $4$ operations in total, we achieve the goal.</p><p>For the third test case, initially $S=\{6\}$. We can apply the following operations:</p><ul> <li> Select $u=6$, remove $u$ from $S$, and insert $1,2,3$ into $S$. Now, $S=\{1,2,3\}$. </li><li> Select $u=2$, remove $u$ from $S$, and insert $1,1$ into $S$. Now, $S=\{1,1,1,3\}$. </li><li> Select $u=3$, remove $u$ from $S$, and insert $1,1,1$ into $S$. Now, $S=\{1,1,1,1,1,1\}$. </li></ul><p>Using $3$ operations in total, we achieve the goal.</p><p>For the fourth test case, initially $S=\{16\}$. We can apply the following operations:</p><ul> <li> Select $u=16$, remove $u$ from $S$, and insert $4,4,4,4$ into $S$. Now, $S=\{4,4,4,4\}$. </li><li> Repeat for $4$ times: select $u=4$, remove $u$ from $S$, and insert $1,1,1,1$ into $S$. </li></ul><p>Using $5$ operations in total, we achieve the goal.</p>
