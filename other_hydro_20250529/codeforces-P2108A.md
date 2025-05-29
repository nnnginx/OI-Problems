## Description

<div><p> </p><p>For a permutation $p$ of length $n$$^{\text{∗}}$, we define the function:</p><p>$$ f(p) = \sum_{i=1}^{n} \lvert p_i - i \rvert $$</p><p>You are given a number $n$. You need to compute how many <span class="tex-font-style-bf">distinct</span> values the function $f(p)$ can take when considering <span class="tex-font-style-bf">all possible</span> permutations of the numbers from $1$ to $n$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array). </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 500$)&nbsp;— the number of numbers in the permutations.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of distinct values of the function $f(p)$ for the given length of permutations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 500$)&nbsp;— the number of numbers in the permutations.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of distinct values of the function $f(p)$ for the given length of permutations.</p>





```input1|2,4,6
5
2
3
8
15
43
```




```output1
2
3
17
57
463
```



## Note

<p>Consider the first two examples of the input.</p><p>For $n = 2$, there are only $2$ permutations&nbsp;— $[1, 2]$ and $[2, 1]$. $f([1, 2]) = \lvert 1 - 1 \rvert + \lvert 2 - 2 \rvert = 0$, $f([2, 1]) = \lvert 2 - 1 \rvert + \lvert 1 - 2 \rvert = 1 + 1 = 2$. Thus, the function takes $2$ distinct values.</p><p>For $n=3$, there are already $6$ permutations: $[1, 2, 3]$, $[1, 3, 2]$, $[2, 1, 3]$, $[2, 3, 1]$, $[3, 1, 2]$, $[3, 2, 1]$, the function values of which will be $0, 2, 2, 4, 4$, and $4$ respectively, meaning there are a total of $3$ values.</p>
