## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">3, 2, 1, ... We are the ！ RiOI Team!</span></div><div class="epigraph-source">！ Felix &amp; All, <span class="tex-font-style-it"><a href="https://www.luogu.com.cn/problem/T351681">Special Thanks 3</a></span></div></div><ul> <li> <span class="tex-font-style-it">Peter: Good news: My problem T311013 is approved!</span> </li><li> <span class="tex-font-style-it">$\delta$: I'm glad my computer had gone out of battery so that I wouldn't have participated in wyrqwq's round and gained a negative delta.</span> </li><li> <span class="tex-font-style-it">Felix: [thumbs_up] The problem statement concerning a removed song!</span> </li><li> <span class="tex-font-style-it">Aquawave: Do I mourn my Chemistry?</span> </li><li> <span class="tex-font-style-it">E.Space: ahh?</span> </li><li> <span class="tex-font-style-it">Trine: Bread.</span> </li><li> <span class="tex-font-style-it">Iris: So why am I always testing problems?</span> </li></ul><p><span class="tex-font-style-it">Time will pass, and we might meet again. Looking back at the past, everybody has lived the life they wanted.</span></p><p>Aquawave has a matrix $A$ of size $n\times m$, whose elements can only be integers in the range $[1, k]$, inclusive. In the matrix, some cells are already filled with an integer, while the rest are currently not filled, denoted by $-1$.</p><p>You are going to fill in all the unfilled places in $A$. After that, let $c_{u,i}$ be the number of occurrences of element $u$ in the $i$-th row. Aquawave defines the <span class="tex-font-style-it">beauty</span> of the matrix as</p><p>$$\sum_{u=1}^k \sum_{i=1}^{n-1} c_{u,i} \cdot c_{u,i+1}.$$</p><p>You have to find the maximum possible beauty of $A$ after filling in the blanks optimally.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \leq n \leq 2\cdot 10^5$, $2 \leq m \leq 2\cdot 10^5$, $n \cdot m \leq 6\cdot 10^5$, $1 \leq k \leq n\cdot m$)&nbsp;！ the number of rows and columns of the matrix $A$, and the range of the integers in the matrix, respectively.</p><p>Then $n$ lines follow, the $i$-th line containing $m$ integers $A_{i,1},A_{i,2},\ldots,A_{i,m}$ ($1 \leq A_{i,j} \leq k$ or $A_{i,j} = -1$) ！ the elements in $A$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $6\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer ！ the maximum possible beauty.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 2\cdot 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \leq n \leq 2\cdot 10^5$, $2 \leq m \leq 2\cdot 10^5$, $n \cdot m \leq 6\cdot 10^5$, $1 \leq k \leq n\cdot m$)&nbsp;！ the number of rows and columns of the matrix $A$, and the range of the integers in the matrix, respectively.</p><p>Then $n$ lines follow, the $i$-th line containing $m$ integers $A_{i,1},A_{i,2},\ldots,A_{i,m}$ ($1 \leq A_{i,j} \leq k$ or $A_{i,j} = -1$) ！ the elements in $A$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $6\cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer ！ the maximum possible beauty.</p>





```input1|2,3,4,5,9,10,11,12,17,18,19,20,21,22,30,31,32,33,34,35,36,43,44,45,46,47,48,49
9
3 3 3
1 2 2
3 1 3
3 2 1
2 3 3
-1 3 3
2 2 -1
3 3 6
-1 -1 1
1 2 -1
-1 -1 4
3 4 5
1 3 2 3
-1 -1 2 -1
3 1 5 1
5 3 8
5 -1 2
1 8 -1
-1 5 6
7 7 -1
4 4 4
6 6 5
-1 -1 5 -1 -1 -1
-1 -1 -1 -1 2 -1
-1 1 3 3 -1 -1
-1 1 -1 -1 -1 4
4 2 -1 -1 -1 4
-1 -1 1 2 -1 -1
6 6 4
-1 -1 -1 -1 1 -1
3 -1 2 2 4 -1
3 1 2 2 -1 -1
3 3 3 3 -1 2
-1 3 3 -1 1 3
3 -1 2 2 3 -1
5 5 3
1 1 3 -1 1
2 2 -1 -1 3
-1 -1 -1 2 -1
3 -1 -1 -1 2
-1 1 2 3 -1
6 2 7
-1 7
-1 6
7 -1
-1 -1
-1 -1
2 2
```




```output1
4
4
10
10
8
102
93
58
13
```



## Note

<p>In the first test case, the matrix $A$ is already determined. Its beauty is</p><p>$$\sum_{u=1}^k \sum_{i=1}^{n-1} c_{u,i} \cdot c_{u,i+1} = c_{1,1}\cdot c_{1,2} + c_{1,2}\cdot c_{1,3} + c_{2,1}\cdot c_{2,2} + c_{2,2}\cdot c_{2,3} + c_{3,1}\cdot c_{3,2} + c_{3,2}\cdot c_{3,3} = 1\cdot 1 + 1\cdot 1 + 2\cdot 0 + 0\cdot 1 + 0\cdot 2 + 2\cdot 1 = 4.$$</p><p>In the second test case, one can fill the matrix as follows:</p><p>$$ \begin{bmatrix} 2 &amp;3 &amp;3 \\ 2 &amp;2 &amp;3 \end{bmatrix}, $$</p><p>and get the value $4$. It can be proven this is the maximum possible answer one can get.</p><p>In the third test case, one of the possible optimal configurations is:</p><p>$$ \begin{bmatrix} 1 &amp;1 &amp;1 \\ 1 &amp;2 &amp;1 \\ 1 &amp;1 &amp;4 \end{bmatrix}. $$</p><p>In the fourth test case, one of the possible optimal configurations is:</p><p>$$ \begin{bmatrix} 1 &amp;3 &amp;2 &amp;3 \\ 1 &amp;3 &amp;2 &amp;1 \\ 3 &amp;1 &amp;5 &amp;1 \end{bmatrix}. $$</p><p>In the fifth test case, one of the possible optimal configurations is:</p><p>$$ \begin{bmatrix} 5 &amp;5 &amp;2 \\ 1 &amp;8 &amp;5 \\ 7 &amp;5 &amp;6 \\ 7 &amp;7 &amp;4 \\ 4 &amp;4 &amp;4 \end{bmatrix}. $$</p>
