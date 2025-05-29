## Description

<div><p><span class="tex-font-style-bf">This is an easy version of the problem; it differs from the hard version only by the question. The easy version only needs you to print whether some values are non-zero or not. The hard version needs you to print the exact values.</span></p><p>Alice and Bob are dividing the field. The field is a rectangle of size $n \times m$ ($2 \le n, m \le 10^9$), the rows are numbered from $1$ to $n$ from top to bottom, and the columns are numbered from $1$ to $m$ from left to right. The cell at the intersection of row $r$ and column $c$ is denoted as ($r, c$).</p><p>Bob has $k$ ($2 \le k \le 2 \cdot 10^5$) fountains, all of them are located in different cells of the field. Alice is responsible for dividing the field, but she must meet several conditions:</p><ul> <li> To divide the field, Alice will start her path in any free (without a fountain) cell on the left or top side of the field and will move, each time moving to the adjacent cell <span class="tex-font-style-bf">down</span> or <span class="tex-font-style-bf">right</span>. Her path will end on the right or bottom side of the field. </li><li> Alice's path will divide the field into two parts ！ one part will belong to Alice (this part includes the cells of her path), the other part ！ to Bob. </li><li> Alice will own the part that includes the cell ($n, 1$). </li><li> Bob will own the part that includes the cell ($1, m$). </li></ul><p>Alice wants to divide the field in such a way as to get as many cells as possible.</p><p>Bob wants to keep ownership of all the fountains, but he can give one of them to Alice. First, output the integer $\alpha$ ！ the maximum possible size of Alice's plot, if Bob does not give her any fountain (i.e., all fountains will remain on Bob's plot). Then output $k$ non-negative integers $a_1, a_2, \dots, a_k$, where:</p><ul> <li> $a_i=0$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot does not increase (i.e., remains equal to $\alpha$); </li><li> $a_i=1$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot increases (i.e., becomes greater than $\alpha$). </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \le n, m \le 10^9$, $2 \le k \le 2 \cdot 10^5$)&nbsp;！ the field sizes and the number of fountains, respectively.</p><p>Then follow $k$ lines, each containing two numbers $r_i$ and $c_i$ ($1 \le r_i \le n$, $1 \le c_i \le m$)&nbsp;！ the coordinates of the cell with the $i$-th fountain. It is guaranteed that all cells are distinct and none of them is ($n, 1$).</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, first output $\alpha$&nbsp;！ the maximum size of the plot that can belong to Alice if Bob does not give her any of the fountains. Then output $k$ non-negative integers $a_1, a_2, \dots, a_k$, where:</p><ul> <li> $a_i=0$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot does not increase compared to the case when all $k$ fountains belong to Bob; </li><li> $a_i=1$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot increases compared to the case when all $k$ fountains belong to Bob. </li></ul><p><span class="tex-font-style-bf">If you output any other positive number instead of $1$ that fits into a 64-bit signed integer type, it will also be recognized as $1$. Thus, a solution to the hard version of this problem will also pass the tests for the easy version.</span></p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \le n, m \le 10^9$, $2 \le k \le 2 \cdot 10^5$)&nbsp;！ the field sizes and the number of fountains, respectively.</p><p>Then follow $k$ lines, each containing two numbers $r_i$ and $c_i$ ($1 \le r_i \le n$, $1 \le c_i \le m$)&nbsp;！ the coordinates of the cell with the $i$-th fountain. It is guaranteed that all cells are distinct and none of them is ($n, 1$).</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, first output $\alpha$&nbsp;！ the maximum size of the plot that can belong to Alice if Bob does not give her any of the fountains. Then output $k$ non-negative integers $a_1, a_2, \dots, a_k$, where:</p><ul> <li> $a_i=0$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot does not increase compared to the case when all $k$ fountains belong to Bob; </li><li> $a_i=1$, if after Bob gives Alice the $i$-th fountain, the maximum possible size of Alice's plot increases compared to the case when all $k$ fountains belong to Bob. </li></ul><p><span class="tex-font-style-bf">If you output any other positive number instead of $1$ that fits into a 64-bit signed integer type, it will also be recognized as $1$. Thus, a solution to the hard version of this problem will also pass the tests for the easy version.</span></p>





```input1|2,3,4,5,11,12,13,14,15,16,17,18,19,20,26,27,28,29,30,31
5
2 2 3
1 1
1 2
2 2
5 5 4
1 2
2 2
3 4
4 3
2 5 9
1 2
1 5
1 1
2 2
2 4
2 5
1 4
2 3
1 3
6 4 4
6 2
1 3
1 4
1 2
3 4 5
2 1
3 2
1 4
1 3
2 4
```




```output1
1
1 0 1 
11
0 1 0 1 
1
0 0 1 1 0 0 0 0 0 
6
1 0 0 0 
1
1 1 0 0 0
```



## Note

<p>Below are the images for the second example: </p><center> <img class="tex-graphics" src="./34712/file/HuWAKdr6.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The indices of the fountains are labeled in green. The cells belonging to Alice are marked in blue.</span> </center><p>Note that if Bob gives Alice fountain $1$ or fountain $3$, then that fountain cannot be on Alice's plot.</p>
