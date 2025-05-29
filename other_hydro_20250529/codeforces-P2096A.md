## Description

<div><p>You are the proud owner of $n$ sticks. Each stick has an integer length from $1$ to $n$. The lengths of the sticks are <span class="tex-font-style-bf">distinct</span>.</p><p>You want to arrange the sticks in a row. There is a string $s$ of length $n - 1$ that describes the requirements of the arrangement.</p><p>Specifically, for each $i$ from $1$ to $n - 1$:</p><ul><li> If $s_i = \texttt{&lt;}$, then the length of the stick at position $i + 1$ must be <span class="tex-font-style-bf">smaller</span> than all sticks before it; </li><li> If $s_i = \texttt{&gt;}$, then the length of the stick at position $i + 1$ must be <span class="tex-font-style-bf">larger</span> than all sticks before it.</li></ul><p>Find any valid arrangement of sticks. We can show that an answer always exists.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$)&nbsp;！ the number of sticks.</p><p>The second line of each test case contains a single string $s$ of length $n - 1$ consisting of characters $\texttt{&lt;}$ and $\texttt{&gt;}$&nbsp;！ describing the requirements of the arrangement.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$, the $a_i$ are distinct)&nbsp;！ the lengths of the sticks in order. If there are multiple solutions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 100$)&nbsp;！ the number of sticks.</p><p>The second line of each test case contains a single string $s$ of length $n - 1$ consisting of characters $\texttt{&lt;}$ and $\texttt{&gt;}$&nbsp;！ describing the requirements of the arrangement.</p>

## Output

<p>For each test case, output $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$, the $a_i$ are distinct)&nbsp;！ the lengths of the sticks in order. If there are multiple solutions, print any of them.</p>





```input1|2,3,6,7,10,11
5
2
&lt;
5
&lt;&lt;&gt;&lt;
2
&gt;
3
&lt;&gt;
7
&gt;&lt;&gt;&gt;&gt;&lt;
```




```output1
2 1 
4 3 2 5 1 
1 2 
2 1 3 
3 4 2 5 6 7 1
```



## Note

<p>For the first test case, the requirements of the arrangement are as follows:</p><ul><li> $s_1 = \texttt{&lt;}$, which means $a_2$ is smaller than $a_1$.</li></ul><p>Thus, one possible arrangement is $[2, 1]$.</p><p>For the second test case, the requirements of the arrangement are as follows:</p><ul><li> $s_1 = \texttt{&lt;}$, which means $a_2$ is smaller than $a_1$; </li><li> $s_2 = \texttt{&lt;}$, which means $a_3$ is smaller than $a_1$ and $a_2$; </li><li> $s_3 = \texttt{&gt;}$, which means $a_4$ is larger than $a_1$, $a_2$, and $a_3$; </li><li> $s_4 = \texttt{&lt;}$, which means $a_5$ is smaller than $a_1$, $a_2$, $a_3$, and $a_4$.</li></ul><p>Thus, one possible arrangement is $[4, 3, 2, 5, 1]$.</p>
