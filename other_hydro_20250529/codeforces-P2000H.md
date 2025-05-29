## Description

<div><p>Ksyusha decided to start a game development company. To stand out among competitors and achieve success, she decided to write her own game engine. The engine must support a set initially consisting of $n$ distinct integers $a_1, a_2, \ldots, a_n$.</p><p>The set will undergo $m$ operations sequentially. The operations can be of the following types: </p><ul> <li> Insert element $x$ into the set; </li><li> Remove element $x$ from the set; </li><li> Report the $k$-load of the set. </li></ul><p>The $k$-load of the set is defined as the <span class="tex-font-style-bf">minimum</span> <span class="tex-font-style-bf">positive</span> integer $d$ such that the integers $d, d + 1, \ldots, d + (k - 1)$ do not appear in this set. For example, the $3$-load of the set $\{3, 4, 6, 11\}$ is $7$, since the integers $7, 8, 9$ are absent from the set, and no smaller value fits.</p><p>Ksyusha is busy with management tasks, so you will have to write the engine. Implement efficient support for the described operations.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following lines describe the test cases.</p><p>The first line contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the initial size of the set.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \ldots &lt; a_n \le 2 \cdot 10^6$)&nbsp;！ the initial state of the set.</p><p>The third line contains an integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;！ the number of operations.</p><p>The next $m$ lines contain the operations. The operations are given in the following format: </p><ul> <li> <span class="tex-font-style-tt">+</span> $x$ ($1 \le x \le 2 \cdot 10^6$)&nbsp;！ insert element $x$ into the set (it is guaranteed that $x$ is not in the set); </li><li> <span class="tex-font-style-tt">-</span> $x$ ($1 \le x \le 2 \cdot 10^6$)&nbsp;！ remove element $x$ from the set (it is guaranteed that $x$ is in the set); </li><li> <span class="tex-font-style-tt">?</span> $k$ ($1 \le k \le 2 \cdot 10^6$)&nbsp;！ output the value of the $k$-load of the set. </li></ul><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$, and the same holds for $m$.</p></div><div class="output-specification"><p>For each test case, output the answers to the operations of type "<span class="tex-font-style-tt">?</span>".</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The following lines describe the test cases.</p><p>The first line contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the initial size of the set.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_1 &lt; a_2 &lt; \ldots &lt; a_n \le 2 \cdot 10^6$)&nbsp;！ the initial state of the set.</p><p>The third line contains an integer $m$ ($1 \le m \le 2 \cdot 10^5$)&nbsp;！ the number of operations.</p><p>The next $m$ lines contain the operations. The operations are given in the following format: </p><ul> <li> <span class="tex-font-style-tt">+</span> $x$ ($1 \le x \le 2 \cdot 10^6$)&nbsp;！ insert element $x$ into the set (it is guaranteed that $x$ is not in the set); </li><li> <span class="tex-font-style-tt">-</span> $x$ ($1 \le x \le 2 \cdot 10^6$)&nbsp;！ remove element $x$ from the set (it is guaranteed that $x$ is in the set); </li><li> <span class="tex-font-style-tt">?</span> $k$ ($1 \le k \le 2 \cdot 10^6$)&nbsp;！ output the value of the $k$-load of the set. </li></ul><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$, and the same holds for $m$.</p>

## Output

<p>For each test case, output the answers to the operations of type "<span class="tex-font-style-tt">?</span>".</p>





```input1|2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,32,33,34,35,36,37,38,39,40,41,42,43,44
3
5
1 2 5 905 2000000
15
- 2
? 2
? 1
- 1
? 1
+ 4
+ 2
? 2
+ 6
- 4
+ 7
? 2
? 3
? 4
? 2000000
5
3 4 5 6 8
9
? 5
- 5
? 5
+ 1
? 2
- 6
- 8
+ 6
? 5
5
6 7 8 9 10
10
? 5
- 6
? 4
- 10
+ 5
- 8
+ 3
+ 2
- 3
+ 10
```




```output1
2 2 1 6 3 8 8 2000001 
9 9 9 7 
1 1
```


