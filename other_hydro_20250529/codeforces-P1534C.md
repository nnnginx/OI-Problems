## Description

<div><p>When he's not training for IOI, Little Alawn enjoys playing with puzzles of various types to stimulate his brain. Today, he's playing with a puzzle that consists of a $2 \times n$ grid where each row is a permutation of the numbers $1,2,3,\ldots,n$.</p><p>The goal of Little Alawn's puzzle is to make sure no numbers on the same column or row are the same (we'll call this state of the puzzle as solved), and to achieve this he is able to swap the numbers in any column. However, after solving the puzzle many times, Little Alawn got bored and began wondering about the number of possible solved configurations of the puzzle he could achieve from an initial <span class="tex-font-style-bf">solved</span> configuration only by swapping numbers in a column.</p><p>Unfortunately, Little Alawn got stuck while trying to solve this harder problem, so he was wondering if you could help him with it. Find the answer modulo $10^9+7$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$).</p><p>The next two lines of each test case describe the initial state of the puzzle grid. Each line will be a permutation of the numbers $1,2,3,\ldots,n$ and the numbers in each column and row will be pairwise distinct.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer, the number of possible solved configurations of the puzzle Little Alawn can achieve from an initial solved configuration only by swapping numbers in a column. As the answer can be very large, please output it modulo $10^9+7$.</p><p>The answer for each test case should be on a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$).</p><p>The next two lines of each test case describe the initial state of the puzzle grid. Each line will be a permutation of the numbers $1,2,3,\ldots,n$ and the numbers in each column and row will be pairwise distinct.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case output a single integer, the number of possible solved configurations of the puzzle Little Alawn can achieve from an initial solved configuration only by swapping numbers in a column. As the answer can be very large, please output it modulo $10^9+7$.</p><p>The answer for each test case should be on a separate line.</p>

## Samples

```input1
2
4
1 4 2 3
3 2 1 4
8
2 6 5 1 4 3 7 8
3 8 7 5 1 2 4 6
```

```output1
2
8
```




## Note

<p>The two possible puzzle configurations for example $1$ are:</p><ul> <li> $[1,4,2,3]$ in the first row and $[3,2,1,4]$ in the second; </li><li> $[3,2,1,4]$ in the first row and $[1,4,2,3]$ in the second. </li></ul>
