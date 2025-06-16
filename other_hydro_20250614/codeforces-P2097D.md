## Description

<div><p>Some teachers work at the educational center "Sirius" while simultaneously studying at the university. In this case, the trip does not exempt them from completing their homework, so they do their homework right on the plane. Artem is one of those teachers, and he was assigned the following homework at the university.</p><p>With an arbitrary string $a$ of <span class="tex-font-style-bf">even</span> length $m$, he can perform the following operation. Artem splits the string $a$ into two halves $x$ and $y$ of equal length, after which he performs <span class="tex-font-style-bf">exactly one</span> of three actions: </p><ul> <li> For each $i \in \left\{ 1, 2, \ldots, \frac{m}{2}\right\}$ assign $x_i = (x_i + y_i) \bmod 2$; </li><li> For each $i \in \left\{ 1, 2, \ldots, \frac{m}{2}\right\}$ assign $y_i = (x_i + y_i) \bmod 2$; </li><li> Perform an arbitrary number of operations (the same operations defined above, applied recursively) on the strings $x$ and $y$, independently of each other. Note that in this case, the strings $x$ and $y$ must be of even length. </li></ul> After that, the string $a$ is replaced by the strings $x$ and $y$, concatenated in the same order.<p>Unfortunately, Artem fell asleep on the plane, so you will have to complete his homework. Artem has two binary strings $s$ and $t$ of length $n$, each consisting of $n$ characters <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. Determine whether it is possible to make string $s$ equal to string $t$ with <span class="tex-font-style-bf">an arbitrary</span> number of operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$) ¡ª the length of the strings $s$ and $t$.</p><p>The second line of each test case contains the string $s$ of length $n$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line of each test case contains the string $t$ of length $n$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it is possible to make string $s$ equal to string $t$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$) ¡ª the length of the strings $s$ and $t$.</p><p>The second line of each test case contains the string $s$ of length $n$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The third line of each test case contains the string $t$ of length $n$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it is possible to make string $s$ equal to string $t$, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,3,4,8,9,10
3
8
00001001
10101001
8
00000000
00001001
6
010110
100010
```




```output1
Yes
No
Yes
```



## Note

<p>In the first test case, the string <span class="tex-font-style-tt">00001001</span> can be transformed into the string <span class="tex-font-style-tt">10101001</span> in two operations. The sequence of actions is illustrated in the figure below:</p><center>  <img class="tex-graphics" src="./37154/file/m2G0VGEG.png" style="max-width: 100.0%;max-height: 100.0%;" width="270px"> </center><p>In the second test case, the string <span class="tex-font-style-tt">00000000</span> cannot be transformed into any string other than <span class="tex-font-style-tt">00000000</span>, as no non-zero elements can be formed during any operation.</p>
