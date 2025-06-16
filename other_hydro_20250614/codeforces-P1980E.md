## Description

<div><p>You have been given a matrix $a$ of size $n$ by $m$, containing a permutation of integers from $1$ to $n \cdot m$.</p><p>A permutation of $n$ integers is an array containing all numbers from $1$ to $n$ exactly once. For example, the arrays $[1]$, $[2, 1, 3]$, $[5, 4, 3, 2, 1]$ are permutations, while the arrays $[1, 1]$, $[100]$, $[1, 2, 4, 5]$ are not.</p><p>A matrix contains a permutation if, when all its elements are written out, the resulting array is a permutation. Matrices $[[1, 2], [3, 4]]$, $[[1]]$, $[[1, 5, 3], [2, 6, 4]]$ contain permutations, while matrices $[[2]]$, $[[1, 1], [2, 2]]$, $[[1, 2], [100, 200]]$ do not.</p><p>You can perform one of the following two actions in one operation:</p><ul> <li> choose columns $c$ and $d$ ($1 \le c, d \le m$, $c \ne d$) and swap these columns; </li><li> choose rows $c$ and $d$ ($1 \le c, d \le n$, $c \ne d$) and swap these rows. </li></ul><p>You can perform any number of operations.</p><p>You are given the original matrix $a$ and the matrix $b$. Your task is to determine whether it is possible to transform matrix $a$ into matrix $b$ using the given operations.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case description contains $2$ integers $n$ and $m$ ($1 \le n, m \le n \cdot m \le 2 \cdot 10^5$) ！ the sizes of the matrix.</p><p>The next $n$ lines contain $m$ integers $a_{ij}$ each ($1 \le a_{ij} \le n \cdot m$). It is guaranteed that matrix $a$ is a permutation.</p><p>The next $n$ lines contain $m$ integers $b_{ij}$ each ($1 \le b_{ij} \le n \cdot m$). It is guaranteed that matrix $b$ is a permutation.</p><p>It is guaranteed that the sum of the values $n \cdot m$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the second matrix can be obtained from the first, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) ！ the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case description contains $2$ integers $n$ and $m$ ($1 \le n, m \le n \cdot m \le 2 \cdot 10^5$) ！ the sizes of the matrix.</p><p>The next $n$ lines contain $m$ integers $a_{ij}$ each ($1 \le a_{ij} \le n \cdot m$). It is guaranteed that matrix $a$ is a permutation.</p><p>The next $n$ lines contain $m$ integers $b_{ij}$ each ($1 \le b_{ij} \le n \cdot m$). It is guaranteed that matrix $b$ is a permutation.</p><p>It is guaranteed that the sum of the values $n \cdot m$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" if the second matrix can be obtained from the first, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output each letter in any case (lowercase or uppercase). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be accepted as a positive answer.</p>





```input1|2,3,4,10,11,12,13,14,22,23,24,25,26,27,28,34,35,36
7
1 1
1
1
2 2
1 2
3 4
4 3
2 1
2 2
1 2
3 4
4 3
1 2
3 4
1 5 9 6
12 10 4 8
7 11 3 2
1 5 9 6
12 10 4 8
7 11 3 2
3 3
1 5 9
6 4 2
3 8 7
9 5 1
2 4 6
7 8 3
2 3
1 2 6
5 4 3
6 1 2
3 4 5
1 5
5 1 2 3 4
4 2 5 1 3
```




```output1
YES
YES
NO
YES
YES
NO
YES
```



## Note

<p>In the second example, the original matrix looks like this:</p><p>$ \begin{pmatrix} 1 &amp; 2 \\ 3 &amp; 4 \end{pmatrix} $</p><p>By swapping rows $1$ and $2$, it becomes:</p><p>$ \begin{pmatrix} 3 &amp; 4 \\ 1 &amp; 2 \end{pmatrix} $</p><p>By swapping columns $1$ and $2$, it becomes equal to matrix $b$:</p><p>$ \begin{pmatrix} 4 &amp; 3 \\ 2 &amp; 1 \end{pmatrix} $</p>
