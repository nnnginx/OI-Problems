## Description

<div><p>Recently, the first-year student Maxim learned about the Collatz conjecture, but he didn't pay much attention during the lecture, so he believes that the following process is mentioned in the conjecture:</p><p>There is a variable $x$ and a constant $y$. The following operation is performed $k$ times: </p><ul> <li> increase $x$ by $1$, then </li><li> while the number $x$ is divisible by $y$, divide it by $y$. </li></ul> Note that both of these actions are performed sequentially within one operation.<p>For example, if the number $x = 16$, $y = 3$, and $k = 2$, then after one operation $x$ becomes $17$, and after another operation $x$ becomes $2$, because after adding one, $x = 18$ is divisible by $3$ twice.</p><p>Given the initial values of $x$, $y$, and $k$, Maxim wants to know what is the final value of $x$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The only line of each test case contains three integers $x$, $y$, and $k$ ($1 \le x, k \le 10^{9}$, $2 \le y \le 10^{9}$)&nbsp;！ the initial variable, constant and the number of operations.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the number obtained after applying $k$ operations.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The only line of each test case contains three integers $x$, $y$, and $k$ ($1 \le x, k \le 10^{9}$, $2 \le y \le 10^{9}$)&nbsp;！ the initial variable, constant and the number of operations.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the number obtained after applying $k$ operations.</p>





```input1|2,4,6,8,10,12,14
13
1 3 1
2 3 1
24 5 5
16 3 2
2 2 1
1337 18 1
1 2 144133
12345678 3 10
998244353 2 998244353
998244353 123456789 998244352
998244354 998241111 998244352
998244355 2 9982443
1000000000 1000000000 1000000000
```




```output1
2
1
1
2
3
1338
1
16936
1
21180097
6486
1
2
```



## Note

<p>In the first test case, there is only one operation applied to $x = 1$, resulting in $x$ becoming $2$.</p><p>In the second test case, for $x = 2$, within one operation, one is added to $x$ and it's divided by $y = 3$, resulting in $x$ becoming $1$.</p><p>In the third test case, $x$ changes as follows:</p><ul> <li> After the first operation, $x = 1$, because $24 + 1 = 25$ and $25$ is divisible by $y = 5$ twice within one operation. </li><li> After the second operation, $x = 2$. </li><li> After the third operation, $x = 3$. </li><li> After the fourth operation, $x = 4$. </li><li> After the fifth operation, $x = 1$. </li></ul>
