## Description

<div><p>Ecrade has an integer $x$. He will show you this number in the form of a binary number of length $n$.</p><p>There are two kinds of operations.</p><ol> <li> Replace $x$ with $\left\lfloor \dfrac{x}{2}\right\rfloor$, where $\left\lfloor \dfrac{x}{2}\right\rfloor$ is the greatest integer $\le \dfrac{x}{2}$. </li><li> Replace $x$ with $\left\lceil \dfrac{x}{2}\right\rceil$, where $\left\lceil \dfrac{x}{2}\right\rceil$ is the smallest integer $\ge \dfrac{x}{2}$. </li></ol><p>Ecrade will perform several operations until $x$ becomes $1$. Each time, he will independently choose to perform either the first operation or the second operation with probability $\frac{1}{2}$.</p><p>Ecrade wants to know the expected number of operations he will perform to make $x$ equal to $1$, modulo $10^9 + 7$. However, it seems a little difficult, so please help him!</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of $x$ in binary representation.</p><p>The second line of each test case contains a binary string of length $n$: the number $x$ in the binary representation, presented from the most significant bit to the least significant bit. It is guaranteed that the most significant bit of $x$ is $1$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer representing the expected number of operations Ecrade will perform to make $x$ equal to $1$, modulo $10^9+7$.</p><p>Formally, let $M = 10^9+7$. It can be shown that the exact answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$. </p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of $x$ in binary representation.</p><p>The second line of each test case contains a binary string of length $n$: the number $x$ in the binary representation, presented from the most significant bit to the least significant bit. It is guaranteed that the most significant bit of $x$ is $1$.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer representing the expected number of operations Ecrade will perform to make $x$ equal to $1$, modulo $10^9+7$.</p><p>Formally, let $M = 10^9+7$. It can be shown that the exact answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$. </p>





```input1|2,3,6,7
3
3
110
3
100
10
1101001011
```




```output1
500000006
2
193359386
```



## Note

<p>For simplicity, we call the first operation $\text{OPER 1}$ and the second operation $\text{OPER 2}$.</p><p>In the first test case, $x=6$, and there are six possible series of operations:</p><ul> <li> $6 \xrightarrow{\text{OPER 1}} 3 \xrightarrow{\text{OPER 1}} 1$, the probability is $\dfrac{1}{4}$. </li><li> $6 \xrightarrow{\text{OPER 1}} 3 \xrightarrow{\text{OPER 2}} 2 \xrightarrow{\text{OPER 1}} 1$, the probability is $\dfrac{1}{8}$. </li><li> $6 \xrightarrow{\text{OPER 1}} 3 \xrightarrow{\text{OPER 2}} 2 \xrightarrow{\text{OPER 2}} 1$, the probability is $\dfrac{1}{8}$. </li><li> $6 \xrightarrow{\text{OPER 2}} 3 \xrightarrow{\text{OPER 1}} 1$, the probability is $\dfrac{1}{4}$. </li><li> $6 \xrightarrow{\text{OPER 2}} 3 \xrightarrow{\text{OPER 2}} 2 \xrightarrow{\text{OPER 1}} 1$, the probability is $\dfrac{1}{8}$. </li><li> $6 \xrightarrow{\text{OPER 2}} 3 \xrightarrow{\text{OPER 2}} 2 \xrightarrow{\text{OPER 2}} 1$, the probability is $\dfrac{1}{8}$. </li></ul><p>Thus, the expected number of operations is $2 \cdot \dfrac{1}{4} + 3 \cdot \dfrac{1}{8} + 3 \cdot \dfrac{1}{8} + 2 \cdot \dfrac{1}{4} + 3 \cdot \dfrac{1}{8} + 3 \cdot \dfrac{1}{8} = \dfrac{5}{2} \equiv 500\,000\,006 \pmod{10^9 + 7}$.</p>
