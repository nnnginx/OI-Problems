## Description

<div><p>   </p><p>In an Italian village, a hungry mouse starts at vertex $\textrm{st}$ on a given tree$^{\text{∗}}$ with $n$ vertices.</p><p>Given a permutation $p$ of length $n$$^{\text{†}}$, there are $n$ steps. For the $i$-th step: </p><ul> <li> A tempting piece of Parmesan cheese appears at vertex $p_i$. If the mouse is currently at vertex $p_i$, it will stay there and enjoy the moment. Otherwise, it will move along the simple path to vertex $p_i$ <span class="tex-font-style-bf">by one edge</span>. </li></ul><p>Your task is to find such a permutation so that, after all $n$ steps, the mouse inevitably arrives at vertex $\textrm{en}$, where a trap awaits.</p><p>Note that the mouse must arrive at $\textrm{en}$ after all $n$ steps, though it may pass through $\textrm{en}$ earlier during the process.</p><div class="statement-footnote"><p>$^{\text{∗}}$A tree is a connected graph without cycles. </p><p>$^{\text{†}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $\textrm{st}$, and $\textrm{en}$ ($1 \le n \le 10^5$; $1 \le \textrm{st}, \textrm{en} \le n$)&nbsp;— the number of vertices of the tree, the starting vertex, and the trap vertex.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$)&nbsp;— the indices of the vertices connected by an edge.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p></div><div class="output-specification"><p>For each test case:</p><ul> <li> If no such permutation exists, output $-1$. </li><li> Otherwise, output $n$ integers $p_1, p_2, \ldots, p_n$, representing the order in which the cheese will appear at the vertices, ensuring the mouse will eventually be caught at vertex $\textrm{en}$. </li></ul><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $\textrm{st}$, and $\textrm{en}$ ($1 \le n \le 10^5$; $1 \le \textrm{st}, \textrm{en} \le n$)&nbsp;— the number of vertices of the tree, the starting vertex, and the trap vertex.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$)&nbsp;— the indices of the vertices connected by an edge.</p><p>It is guaranteed that the given edges form a tree.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$. </p>

## Output

<p>For each test case:</p><ul> <li> If no such permutation exists, output $-1$. </li><li> Otherwise, output $n$ integers $p_1, p_2, \ldots, p_n$, representing the order in which the cheese will appear at the vertices, ensuring the mouse will eventually be caught at vertex $\textrm{en}$. </li></ul><p>If there are multiple solutions, print any of them.</p>





```input1|2,5,6,7
4
1 1 1
2 1 2
1 2
3 2 2
1 2
2 3
6 1 4
1 2
1 3
4 5
5 6
1 4
```




```output1
1 
1 2 
3 1 2 
1 4 3 2 6 5
```



## Note

<p>In the first test case, there is only one permutation with length $n = 1$ that is $p = [1]$, which successfully catches the mouse:</p><p>$$\textrm{st} = 1 \overset{p_1 = 1}{\xrightarrow{\hspace{1.3cm}}} 1 = \textrm{en}.$$</p><p>In the second test case, one possible permutation with length $n = 2$ is $p = [1, 2]$:</p><p>$$\textrm{st} = 1 \overset{p_1 = 1}{\xrightarrow{\hspace{1.3cm}}} 1 \overset{p_2 = 2}{\xrightarrow{\hspace{1.3cm}}} 2 = \textrm{en}.$$</p><p>In the third test case, one possible permutation with length $n = 3$ is $p = [3, 1, 2]$:</p><p>$$\textrm{st} = 2 \overset{p_1 = 3}{\xrightarrow{\hspace{1.3cm}}} 3 \overset{p_2 = 1}{\xrightarrow{\hspace{1.3cm}}} 2 \overset{p_3 = 2}{\xrightarrow{\hspace{1.3cm}}} 2 = \textrm{en}.$$</p>
