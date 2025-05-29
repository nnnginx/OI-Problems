## Description

<div><p>Brr Brrr Patapim is trying to learn of Tiramisù's secret passcode, which is a permutation$^{\text{∗}}$ of $2\cdot n$ elements. To help Patapim guess, Tiramisù gave him an $n\times n$ grid $G$, in which $G_{i,j}$ (or the element in the $i$-th row and $j$-th column of the grid) contains $p_{i+j}$, or the $(i+j)$-th element in the permutation. </p><p>Given this grid, please help Patapim crack the forgotten code. It is guaranteed that the permutation exists, and it can be shown that the permutation can be determined uniquely.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of $m$ integers is a sequence of $m$ integers which contains each of $1,2,\ldots,m$ exactly once. For example, $[1, 3, 2]$ and $[2, 1]$ are permutations, while $[1, 2, 4]$ and $[1, 3, 2, 3]$ are not.</p></div></div><div class="input-specification"><p>The first line contains an integer $t$&nbsp;— the number of test cases ($1 \leq t \leq 200$).</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 800$).</p><p>Each of the following $n$ lines contains $n$ integers, giving the grid $G$. The first of these lines contains $G_{1,1}, G_{1,2},\ldots,G_{1,n}$; the second of these lines contains $G_{2,1}, G_{2,2},\ldots,G_{2,n}$, and so on. ($1 \leq G_{i,j} \leq 2\cdot n$).</p><p>It is guaranteed that the grid encodes a valid permutation, and the sum of $n$ over all test cases does not exceed $800$.</p></div><div class="output-specification"><p>For each test case, please output $2n$ numbers on a new line: $p_1,p_2,\ldots,p_{2n}$.</p></div>

## Input

<p>The first line contains an integer $t$&nbsp;— the number of test cases ($1 \leq t \leq 200$).</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 800$).</p><p>Each of the following $n$ lines contains $n$ integers, giving the grid $G$. The first of these lines contains $G_{1,1}, G_{1,2},\ldots,G_{1,n}$; the second of these lines contains $G_{2,1}, G_{2,2},\ldots,G_{2,n}$, and so on. ($1 \leq G_{i,j} \leq 2\cdot n$).</p><p>It is guaranteed that the grid encodes a valid permutation, and the sum of $n$ over all test cases does not exceed $800$.</p>

## Output

<p>For each test case, please output $2n$ numbers on a new line: $p_1,p_2,\ldots,p_{2n}$.</p>





```input1|2,3,4,5,8,9,10
3
3
1 6 2
6 2 4
2 4 3
1
1
2
2 3
3 4
```




```output1
5 1 6 2 4 3 
2 1 
1 2 3 4
```


