## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/user-838515264/camellia-parts-ooparts">ΩΩPARTS - Camellia</a></span></div><div class="epigraph-source">⠀</div></div><p>Farmer John has an array $a$ of length $n$. He also has a function $f$ with the following recurrence: </p><ul> <li> $f(1) = \sqrt{a_1}$; </li><li> For all $i &gt; 1$, $f(i) = \sqrt{f(i-1)+a_i}$. </li></ul><p>Note that $f(i)$ is not necessarily an integer.</p><p>He plans to do $q$ updates to the array. Each update, he gives you two integers $k$ and $x$ and he wants you to set $a_k = x$. After each update, he wants to know $\lfloor f(n) \rfloor$, where $\lfloor t \rfloor$ denotes the value of $t$ rounded down to the nearest integer.</p></div><div class="input-specification"><p>The first line contains $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$), the length of $a$ and the number of updates he will perform.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^{18}$).</p><p>The next $q$ lines each contain two integers $k$ and $x$ ($1 \leq k \leq n$, $0 \leq x \leq 10^{18}$), the index of the update and the element he will replace $a_k$ with.</p></div><div class="output-specification"><p>For each update, output an integer, $\lfloor f(n) \rfloor$, on a new line.</p></div>

## Input

<p>The first line contains $n$ and $q$ ($1 \leq n, q \leq 2 \cdot 10^5$), the length of $a$ and the number of updates he will perform.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^{18}$).</p><p>The next $q$ lines each contain two integers $k$ and $x$ ($1 \leq k \leq n$, $0 \leq x \leq 10^{18}$), the index of the update and the element he will replace $a_k$ with.</p>

## Output

<p>For each update, output an integer, $\lfloor f(n) \rfloor$, on a new line.</p>





```input1|
5 6
0 14 0 7 6
1 4
1 3
2 15
4 1
5 2
5 8
```




```input2|
15 10
3364 1623 5435 7 6232 245 7903 3880 9738 577 4598 1868 1112 8066 199
14 4284
14 8066
6 92
6 245
2 925
2 1623
5 176
5 6232
3 1157
3 5435
```




```input3|
2 2
386056082462833225 923951085408043421
1 386056082462833225
1 386056082462833224
```




```input4|
13 10
31487697732100 446330174221392699 283918145228010533 619870471872432389 11918456891794188 247842810542459080 140542974216802552 698742782599365547 533363381213535498 92488084424940128 401887157851719898 128798321287952855 137376848358184069
3 283918145228010532
3 283918145228010533
1 2183728930312
13 1000000000000000000
10 1000000000000000000
9 1000000000000000000
8 1000000000000000000
7 1000000000000000000
6 1000000000000000000
5 1000000000000000000
```




```output1
3
2
3
2
1
3
```




```output2
16
17
16
17
16
17
16
17
16
17
```




```output3
961223744
961223743
```




```output4
370643829
370643830
370643829
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
1000000000
```



## Note

<p>In the first test case, the array after the first update is $[4, 14, 0, 7, 6]$. The values of $f$ are:</p><ul> <li> $f(1)=2$; </li><li> $f(2)=4$; </li><li> $f(3)=2$; </li><li> $f(4)=3$; </li><li> $f(5)=3$. </li></ul><p>Since $\lfloor f(5) \rfloor = 3$, we output $3$.</p><p>The array after the second update is $[3, 14, 0, 7, 6]$. The values of $f$, rounded to $6$ decimal places, are:</p><ul> <li> $f(1)\approx 1.732051$; </li><li> $f(2)\approx 3.966365$; </li><li> $f(3)\approx 1.991573$; </li><li> $f(4)\approx 2.998595$; </li><li> $f(5)\approx 2.999766$. </li></ul><p>Since $\lfloor f(5) \rfloor = 2$, we output $2$.</p>
