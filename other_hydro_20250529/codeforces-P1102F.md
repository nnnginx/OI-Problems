## Description

<div><p>You are given a matrix $a$, consisting of $n$ rows and $m$ columns. Each cell contains an integer in it.</p><p>You can change the order of rows arbitrarily (including leaving the initial order), but you can't change the order of cells in a row. After you pick some order of rows, you traverse the whole matrix the following way: firstly visit all cells of the first column from the top row to the bottom one, then the same for the second column and so on. During the traversal you write down the sequence of the numbers on the cells in the same order you visited them. Let that sequence be $s_1, s_2, \dots, s_{nm}$. </p><p>The traversal is $k$-acceptable if for all $i$ ($1 \le i \le nm - 1$) $|s_i - s_{i + 1}| \ge k$.</p><p>Find the maximum integer $k$ such that there exists some order of rows of matrix $a$ that it produces a $k$-acceptable traversal.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 16$, $1 \le m \le 10^4$, $2 \le nm$) ！ the number of rows and the number of columns, respectively.</p><p>Each of the next $n$ lines contains $m$ integers ($1 \le a_{i, j} \le 10^9$) ！ the description of the matrix.</p></div><div class="output-specification"><p>Print a single integer $k$ ！ the maximum number such that there exists some order of rows of matrix $a$ that it produces an $k$-acceptable traversal.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 16$, $1 \le m \le 10^4$, $2 \le nm$) ！ the number of rows and the number of columns, respectively.</p><p>Each of the next $n$ lines contains $m$ integers ($1 \le a_{i, j} \le 10^9$) ！ the description of the matrix.</p>

## Output

<p>Print a single integer $k$ ！ the maximum number such that there exists some order of rows of matrix $a$ that it produces an $k$-acceptable traversal.</p>

## Samples

```input1
4 2
9 9
10 8
5 3
4 3
```

```output1
5
```






```input2
2 4
1 2 3 4
10 3 7 3
```

```output2
0
```






```input3
6 1
3
6
2
5
1
4
```

```output3
3
```




## Note

<p>In the first example you can rearrange rows as following to get the $5$-acceptable traversal:</p><pre class="verbatim">
5 3
10 8
4 3
9 9
</pre><p>Then the sequence $s$ will be $[5, 10, 4, 9, 3, 8, 3, 9]$. Each pair of neighbouring elements have at least $k = 5$ difference between them.</p><p>In the second example the maximum $k = 0$, any order is $0$-acceptable.</p><p>In the third example the given order is already $3$-acceptable, you can leave it as it is.</p>
