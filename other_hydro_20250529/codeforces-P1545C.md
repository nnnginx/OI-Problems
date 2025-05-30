## Description

<div><p>Cirno has prepared $n$ arrays of length $n$ each. Each array is a permutation of $n$ integers from $1$ to $n$. These arrays are special: for all $1 \leq i \leq n$, if we take the $i$-th element of each array and form another array of length $n$ with these elements, the resultant array is also a permutation of $n$ integers from $1$ to $n$. In the other words, if you put these $n$ arrays under each other to form a matrix with $n$ rows and $n$ columns, this matrix is a <a href="https://en.wikipedia.org/wiki/Latin_square">Latin square</a>.</p><p>Afterwards, Cirno added additional $n$ arrays, each array is a permutation of $n$ integers from $1$ to $n$. For all $1 \leq i \leq n$, there exists <span class="tex-font-style-bf">at least one</span> position $1 \leq k \leq n$, such that for the $i$-th array and the $(n + i)$-th array, the $k$-th element of both arrays is the same. Notice that the arrays indexed from $n + 1$ to $2n$ <span class="tex-font-style-bf">don't have to</span> form a Latin square. </p><p>Also, Cirno made sure that for all $2n$ arrays, no two arrays are completely equal, i.&nbsp;e. for all pair of indices $1 \leq i &lt; j \leq 2n$, there exists <span class="tex-font-style-bf">at least one</span> position $1 \leq k \leq n$, such that the $k$-th elements of the $i$-th and $j$-th array are <span class="tex-font-style-bf">different</span>.</p><p>Finally, Cirno arbitrarily changed the order of $2n$ arrays.</p><p>AquaMoon calls a subset of all $2n$ arrays of size $n$ <span class="tex-font-style-bf">good</span> if these arrays from a Latin square.</p><p>AquaMoon wants to know how many good subsets exist. Because this number may be particularly large, find it modulo $998\,244\,353$. Also, she wants to find any good subset. Can you help her?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) ！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($5 \leq n \leq 500$).</p><p>Then $2n$ lines followed. The $i$-th of these lines contains $n$ integers, representing the $i$-th array.</p><p>It is guaranteed, that the sum of $n$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case print two lines.</p><p>In the first line, print the number of good subsets by modulo $998\,244\,353$.</p><p>In the second line, print $n$ indices from $1$ to $2n$ ！ indices of the $n$ arrays that form a good subset (you can print them in any order). If there are several possible answers ！ print any of them.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) ！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($5 \leq n \leq 500$).</p><p>Then $2n$ lines followed. The $i$-th of these lines contains $n$ integers, representing the $i$-th array.</p><p>It is guaranteed, that the sum of $n$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case print two lines.</p><p>In the first line, print the number of good subsets by modulo $998\,244\,353$.</p><p>In the second line, print $n$ indices from $1$ to $2n$ ！ indices of the $n$ arrays that form a good subset (you can print them in any order). If there are several possible answers ！ print any of them.</p>

## Samples

```input1
3
7
1 2 3 4 5 6 7
2 3 4 5 6 7 1
3 4 5 6 7 1 2
4 5 6 7 1 2 3
5 6 7 1 2 3 4
6 7 1 2 3 4 5
7 1 2 3 4 5 6
1 2 3 4 5 7 6
1 3 4 5 6 7 2
1 4 5 6 7 3 2
1 5 6 7 4 2 3
1 6 7 5 2 3 4
1 7 6 2 3 4 5
1 7 2 3 4 5 6
5
4 5 1 2 3
3 5 2 4 1
1 2 3 4 5
5 2 4 1 3
3 4 5 1 2
2 3 4 5 1
1 3 5 2 4
4 1 3 5 2
2 4 1 3 5
5 1 2 3 4
6
2 3 4 5 6 1
3 1 2 6 4 5
6 1 2 3 4 5
5 6 1 3 2 4
4 3 6 5 2 1
5 6 1 2 3 4
4 5 6 1 2 3
3 4 5 6 1 2
1 2 3 4 5 6
2 5 4 1 6 3
3 2 5 4 1 6
1 4 3 6 5 2
```

```output1
1
1 2 3 4 5 6 7
2
1 3 5 6 10
4
1 3 6 7 8 9
```




## Note

<p>In the first test case, the number of good subsets is $1$. The only such subset is the set of arrays with indices $1$, $2$, $3$, $4$, $5$, $6$, $7$.</p><p>In the second test case, the number of good subsets is $2$. They are $1$, $3$, $5$, $6$, $10$ or $2$, $4$, $7$, $8$, $9$.</p>
