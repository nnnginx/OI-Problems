## Description

<div><p><span class="tex-font-style-it">Mouf is bored with themes, so he decided not to use any themes for this problem.</span></p><p>You are given a binary$^{\text{∗}}$ string $s$ of length $n$. You are to perform the following operation exactly $k$ times:</p><ul> <li> select an index $i$ ($1 \le i \le n$) such that $s_i = \mathtt{0}$; </li><li> then flip$^{\text{†}}$ each $s_j$ for all indices $j$ ($1 \le j \le i$). </li></ul><p>You need to count the number of possible ways to perform all $k$ operations. </p><p>Since the answer could be ginormous, print it modulo $998\,244\,353$.</p><p>Two sequences of operations are considered different if they differ in the index selected at any step.</p><div class="statement-footnote"><p>$^{\text{∗}}$A binary string is a string that consists only of the characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>$^{\text{†}}$Flipping a binary character is changing it from $\mathtt{0}$ to $\mathtt{1}$ or vice versa.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 500$)&nbsp;— the length of the binary string $s$ and the number of times the operation must be performed, respectively.</p><p>The second line of each test case contains a binary string $s$ of length $n$ consisting of only characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>It is guaranteed that the sum of $n$ does not exceed $500$ over all test cases.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of ways you can perform exactly $k$ operations, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 500$)&nbsp;— the length of the binary string $s$ and the number of times the operation must be performed, respectively.</p><p>The second line of each test case contains a binary string $s$ of length $n$ consisting of only characters $\mathtt{0}$ and $\mathtt{1}$.</p><p>It is guaranteed that the sum of $n$ does not exceed $500$ over all test cases.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of ways you can perform exactly $k$ operations, modulo $998\,244\,353$.</p>





```input1|2,3,6,7,10,11
5
3 1
010
3 2
000
5 4
01001
8 8
11001100
20 20
10010110101101010110
```




```output1
2
3
10
27286
915530405
```



## Note

<p>In the first test case, here are all the possible sequences of operations: </p><ul> <li> $\mathtt{\color{red}{0}10} \xrightarrow{i = 1} \mathtt{110}$ </li><li> $\mathtt{\color{red}{010}} \xrightarrow{i = 3} \mathtt{101}$ </li></ul><p>In the second test case, here are all the possible sequences of operations: </p><ul> <li> $\mathtt{\color{red}{0}00} \xrightarrow{i = 1} \mathtt{\color{red}{1}00} \xrightarrow{i = 2} \mathtt{010}$ </li><li> $\mathtt{\color{red}{0}00} \xrightarrow{i = 1} \mathtt{\color{red}{1}00} \xrightarrow{i = 3} \mathtt{011}$ </li><li> $\mathtt{\color{red}{00}0} \xrightarrow{i = 2} \mathtt{\color{red}{11}0} \xrightarrow{i = 3} \mathtt{001}$ </li></ul>
