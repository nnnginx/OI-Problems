## Description

<div><p>The sequence of $m$ integers is called the <span class="tex-font-style-it">permutation</span> if it contains all integers from $1$ to $m$ exactly once. The number $m$ is called the length of the permutation.</p><p>Dreamoon has two permutations $p_1$ and $p_2$ of non-zero lengths $l_1$ and $l_2$.</p><p>Now Dreamoon concatenates these two permutations into another sequence $a$ of length $l_1 + l_2$. First $l_1$ elements of $a$ is the permutation $p_1$ and next $l_2$ elements of $a$ is the permutation $p_2$. </p><p>You are given the sequence $a$, and you need to find two permutations $p_1$ and $p_2$. If there are several possible ways to restore them, you should find all of them. (Note that it is also possible that there will be no ways.)</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10\,000$) denoting the number of test cases in the input.</p><p>Each test case contains two lines. The first line contains one integer $n$ ($2 \leq n \leq 200\,000$): the length of $a$. The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n-1$).</p><p>The total sum of $n$ is less than $200\,000$.</p></div><div class="output-specification"><p>For each test case, the first line of output should contain one integer $k$: the number of ways to divide $a$ into permutations $p_1$ and $p_2$.</p><p>Each of the next $k$ lines should contain two integers $l_1$ and $l_2$ ($1 \leq l_1, l_2 \leq n, l_1 + l_2 = n$), denoting, that it is possible to divide $a$ into two permutations of length $l_1$ and $l_2$ ($p_1$ is the first $l_1$ elements of $a$, and $p_2$ is the last $l_2$ elements of $a$). You can print solutions in any order.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10\,000$) denoting the number of test cases in the input.</p><p>Each test case contains two lines. The first line contains one integer $n$ ($2 \leq n \leq 200\,000$): the length of $a$. The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n-1$).</p><p>The total sum of $n$ is less than $200\,000$.</p>

## Output

<p>For each test case, the first line of output should contain one integer $k$: the number of ways to divide $a$ into permutations $p_1$ and $p_2$.</p><p>Each of the next $k$ lines should contain two integers $l_1$ and $l_2$ ($1 \leq l_1, l_2 \leq n, l_1 + l_2 = n$), denoting, that it is possible to divide $a$ into two permutations of length $l_1$ and $l_2$ ($p_1$ is the first $l_1$ elements of $a$, and $p_2$ is the last $l_2$ elements of $a$). You can print solutions in any order.</p>

## Samples

```input1
6
5
1 4 3 2 1
6
2 4 1 3 2 1
4
2 1 1 3
4
1 3 3 1
12
2 1 3 4 5 6 7 8 9 1 10 2
3
1 1 1
```

```output1
2
1 4
4 1
1
4 2
0
0
1
2 10
0
```




## Note

<p>In the first example, two possible ways to divide $a$ into permutations are $\{1\} + \{4, 3, 2, 1\}$ and $\{1,4,3,2\} + \{1\}$.</p><p>In the second example, the only way to divide $a$ into permutations is $\{2,4,1,3\} + \{2,1\}$.</p><p>In the third example, there are no possible ways.</p>
