## Description

<div><p>Given a matrix $a$ of size $n \times m$, each cell of which contains a non-negative integer. The integer lying at the intersection of the $i$-th row and the $j$-th column of the matrix is called $a_{i,j}$.</p><p>Let's define $f(i)$ and $g(j)$ as the <a href="https://en.wikipedia.org/wiki/Exclusive_or">XOR</a> of all integers in the $i$-th row and the $j$-th column, respectively. In one operation, you can either: </p><ul> <li> Select any row $i$, then assign $a_{i,j} := g(j)$ for each $1 \le j \le m$; or </li><li> Select any column $j$, then assign $a_{i,j} := f(i)$ for each $1 \le i \le n$. </li></ul><center> <img class="tex-graphics" src="./34809/file/o9oHP7bA.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">An example of applying an operation on column $2$ of the matrix.</span> </center><p>In this example, as we apply an operation on column $2$, all elements in this column are changed: </p><ul> <li> $a_{1,2} := f(1) = a_{1,1} \oplus a_{1,2} \oplus a_{1,3} \oplus a_{1,4} = 1 \oplus 1 \oplus 1 \oplus 1 = 0$ </li><li> $a_{2,2} := f(2) = a_{2,1} \oplus a_{2,2} \oplus a_{2,3} \oplus a_{2,4} = 2 \oplus 3 \oplus 5 \oplus 7 = 3$ </li><li> $a_{3,2} := f(3) = a_{3,1} \oplus a_{3,2} \oplus a_{3,3} \oplus a_{3,4} = 2 \oplus 0 \oplus 3 \oplus 0 = 1$ </li><li> $a_{4,2} := f(4) = a_{4,1} \oplus a_{4,2} \oplus a_{4,3} \oplus a_{4,4} = 10 \oplus 11 \oplus 12 \oplus 16 = 29$ </li></ul><p>You can apply the operations any number of times. Then, we calculate the $\textit{beauty}$ of the final matrix by summing the absolute differences between all pairs of its adjacent cells.</p><p>More formally, $\textit{beauty}(a) = \sum|a_{x,y} - a_{r,c}|$ for all cells $(x, y)$ and $(r, c)$ if they are adjacent. Two cells are considered adjacent if they share a side.</p><p>Find the minimum $\textit{beauty}$ among all obtainable matrices.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 250$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 15$)&nbsp;！ the number of rows and columns of $a$, respectively.</p><p>The next $n$ lines, each containing $m$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,m}$ ($0 \le a_{i,j} &lt; 2^{20}$)&nbsp;！ description of the matrix $a$.</p><p>It is guaranteed that the sum of $(n^2 + m^2)$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, print a single integer $b$&nbsp;！ the smallest possible $\textit{beauty}$ of the matrix.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 250$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 15$)&nbsp;！ the number of rows and columns of $a$, respectively.</p><p>The next $n$ lines, each containing $m$ integers $a_{i,1}, a_{i,2}, \ldots, a_{i,m}$ ($0 \le a_{i,j} &lt; 2^{20}$)&nbsp;！ description of the matrix $a$.</p><p>It is guaranteed that the sum of $(n^2 + m^2)$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, print a single integer $b$&nbsp;！ the smallest possible $\textit{beauty}$ of the matrix.</p>





```input1|2,3,7,8,9
4
1 2
1 3
2 3
0 1 0
5 4 4
2 3
0 2 4
4 5 1
3 3
1 2 3
4 5 6
7 8 9
```




```output1
1
3
13
24
```



## Note

<p>Let's denote $r(i)$ as the first type operation applied on the $i$-th row, and $c(j)$ as the second type operation applied on the $j$-th column.</p><p>In the first test case, you can apply an operation $c(1)$, which assigns $a_{1,1} := 1 \oplus 3 = 2$. Then, we'll receive this matrix: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td></tr></tbody></table> </center><p>In the second test case, you can apply an operation $r(1)$, which assigns: </p><ul> <li> $a_{1,1} := g(1) = 0 \oplus 5 = 5$ </li><li> $a_{1,2} := g(2) = 1 \oplus 4 = 5$ </li><li> $a_{1,3} := g(3) = 0 \oplus 4 = 4$ </li></ul><p>The resulting matrix after performing the operation is: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td></tr></tbody></table> </center><p>In the third test case, the best way to achieve minimum $\textit{beauty}$ is applying three operations: $c(3)$, $r(2)$, and $c(2)$. The resulting matrix is: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">0</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">6</td></tr></tbody></table> </center>
