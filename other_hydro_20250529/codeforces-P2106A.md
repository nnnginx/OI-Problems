## Description

<div><p>In order to test his patients' intelligence, Dr. TC created the following test.</p><p>First, he creates a binary string$^{\text{∗}}$ $s$ having $n$ characters. Then, he creates $n$ binary strings $a_1, a_2, \ldots, a_n$. It is known that $a_i$ is created by first copying $s$, then flipping the $i$'th character ($\texttt{1}$ becomes $\texttt{0}$ and vice versa). After creating all $n$ strings, he arranges them into a grid where the $i$'th row is $a_i$. </p><p>For example, </p><ul> <li> If $s = \texttt{101}$, $a = [\texttt{001}, \texttt{111}, \texttt{100}]$. </li><li> If $s = \texttt{0000}$, $a = [\texttt{1000}, \texttt{0100}, \texttt{0010}, \texttt{0001}]$. </li></ul><p>The patient needs to count the number of $1$s written on the board in less than a second. Can you pass the test?</p><div class="statement-footnote"><p>$^{\text{∗}}$A binary string is a string that only consists of characters $\texttt{1}$ and $\texttt{0}$.</p></div></div><div class="input-specification"><p>The first line of the input consists of a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10$)&nbsp;— the length of the binary string $s$.</p><p>The second line of each test case contains a single binary string $s$ of size $n$.</p></div><div class="output-specification"><p>For each test case, output a single integer, the number of $\texttt{1}$s on the board.</p></div>

## Input

<p>The first line of the input consists of a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10$)&nbsp;— the length of the binary string $s$.</p><p>The second line of each test case contains a single binary string $s$ of size $n$.</p>

## Output

<p>For each test case, output a single integer, the number of $\texttt{1}$s on the board.</p>





```input1|2,3,6,7,10,11
5
3
101
1
1
5
00000
2
11
3
010
```




```output1
5
0
5
2
4
```



## Note

<p>The first example is explained in the statement.</p><p>For the second example, the only string written on the board will be the string $\texttt{0}$; therefore, the answer is $0$.</p><p>In the third example, the following strings will be written on the board: $[\texttt{10000}, \texttt{01000}, \texttt{00100}, \texttt{00010}, \texttt{00001}]$; so there are five $\texttt{1}$s written on the board.</p>
