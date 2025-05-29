## Description

<div><p><span class="tex-font-style-it">Mouf, the clever master of Darkness, and Fouad, the brave champion of Light, have entered the Grid Realm once more. This time, they have found the exit, but it is guarded by fierce monsters! They must fight with their bare hands instead of summoning monsters!</span></p><p>Mouf and Fouad are standing on an $n \times n$ grid. Each cell $(i, j)$ has a value $a_{i,j}$ and a color. The color of a cell is white if $c_{i,j} = 0$ and black if $c_{i,j} = 1$.</p><p>Mouf starts at the top-left corner $(1, 1)$, and Fouad starts at the bottom-left corner $(n, 1)$. Both are trying to reach the exit cell at $(r, n)$.</p><p>A path is defined as a sequence of adjacent cells (sharing a horizontal or vertical edge). The cost of a path is the maximum value of $a_{i, j}$ among all cells included in the path (including the first and last cells).</p><p>Let: </p><ul> <li> $\mathrm{dis}_M$ denote the minimum possible cost of a valid path from Mouf's starting position $(1, 1)$ to the exit $(r, n)$; </li><li> $\mathrm{dis}_F$ denote the minimum possible cost of a valid path from Fouad's starting position $(n, 1)$ to the exit $(r, n)$. </li></ul><p>Before moving, Mouf can perform up to $k$ operations. In each operation, he may select any black cell and increment its value by $1$ (possibly choosing the same cell multiple times).</p><p>Mouf wants to maximize $\mathrm{dis}_F$ while ensuring that his own cost $\mathrm{dis}_M$ remains <span class="tex-font-style-bf">unchanged</span> (as if he performed no operations). If Mouf acts optimally, what are the values of $\mathrm{dis}_M$ and $\mathrm{dis}_F$?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $r$, and $k$ ($2 \le n \le 300$, $1 \le r \le n$, $0 \le k \le 10^6$)&nbsp;！ the length of the grid, the row number of the exit cell, and the number of allowed operations.</p><p>The $i$-th of the next $n$ lines contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($1 \le a_{ij} \le 10^6$)&nbsp;！ the values of the cells in the $i$-th row.</p><p>The $i$-th of the next $n$ lines contains a binary string $c_i$ of length $n$&nbsp;！ denoting the color of the cells in the $i$-th row (cell $(i,j)$ is white if $c_{i,j}=\mathtt{0}$ and black if $c_{i,j} = \mathtt{1}$).</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $9 \cdot 10^4$.</p></div><div class="output-specification"><p>For each test case, output two integers&nbsp;！ $\mathrm{dis}_M$ and $\mathrm{dis}_F$ if Mouf performs the operations optimally.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $r$, and $k$ ($2 \le n \le 300$, $1 \le r \le n$, $0 \le k \le 10^6$)&nbsp;！ the length of the grid, the row number of the exit cell, and the number of allowed operations.</p><p>The $i$-th of the next $n$ lines contains $n$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,n}$ ($1 \le a_{ij} \le 10^6$)&nbsp;！ the values of the cells in the $i$-th row.</p><p>The $i$-th of the next $n$ lines contains a binary string $c_i$ of length $n$&nbsp;！ denoting the color of the cells in the $i$-th row (cell $(i,j)$ is white if $c_{i,j}=\mathtt{0}$ and black if $c_{i,j} = \mathtt{1}$).</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $9 \cdot 10^4$.</p>

## Output

<p>For each test case, output two integers&nbsp;！ $\mathrm{dis}_M$ and $\mathrm{dis}_F$ if Mouf performs the operations optimally.</p>





```input1|2,3,4,5,6,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28
4
2 1 30
2 2
1 1
11
01
3 3 5
9 2 2
2 3 2
2 2 2
111
111
010
7 3 12
3 3 3 3 5 1 1
9 4 8 3 3 5 5
9 4 8 7 3 3 3
4 4 4 4 9 4 9
4 4 4 4 9 4 9
1 4 4 4 4 4 9
1 1 4 4 9 9 9
1111111
1011111
1011111
1111111
1111101
1110001
0111111
5 3 1419
1219 678 1672 1858 1210
535 732 1316 345 296
1106 3060 507 216 1943
194 2124 47 87 4818
1007 329 1425 284 660
00010
10111
00101
10001
10100
```




```input2|2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18
1
8 2 2216
429 589 675 2022 259 452 733 967
1097 2880 256 1894 259 1052 345 692
911 831 513 1243 200 14 854 217
611 882 681 279 54 719 1469 1885
504 2524 1332 17 3113 34 1281 717
498 1896 1800 2231 731 364 69 1247
1397 399 68 448 1337 1076 166 3786
16 857 91 475 106 102 1517 1949
01010100
00101100
00001000
10100110
00001000
00100000
01100011
00001000
```




```output1
2 2
9 5
3 8
1943 2426
```




```output2
733 1671
```



## Note

<p>In the first test case:</p><ul> <li> Although Mouf can perform up to $30$ operations, he can not increase $\mathrm{dis}_F$ beyond $2$; he is restricted to applying operations only on $(2,2)$, because performing operations on $(1,1)$ or $(1,2)$ would change $\mathrm{dis}_M$. </li><li> Mouf may apply all $30$ operations on cell $(2,2)$; however, Fouad can still follow the path $(2,1) \rightarrow (1,1) \rightarrow (1,2)$ with a cost of $2$. </li></ul><p>In the second test case, Mouf can apply two operations on $(2,2)$ and three operations on $(3,2)$. It can be shown that Mouf can not increase $\mathrm{dis}_F$ beyond $5$.</p>
