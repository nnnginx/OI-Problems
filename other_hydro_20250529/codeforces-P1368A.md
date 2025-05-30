## Description

<div><p>Leo has developed a new programming language C+=. In C+=, integer variables can only be changed with a "<span class="tex-font-style-tt">+=</span>" operation that adds the right-hand side value to the left-hand side variable. For example, performing "<span class="tex-font-style-tt">a += b</span>" when <span class="tex-font-style-tt">a = </span>$2$, <span class="tex-font-style-tt">b = </span>$3$ changes the value of <span class="tex-font-style-tt">a</span> to $5$ (the value of <span class="tex-font-style-tt">b</span> does not change).</p><p>In a prototype program Leo has two integer variables <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>, initialized with some positive values. He can perform any number of operations "<span class="tex-font-style-tt">a += b</span>" or "<span class="tex-font-style-tt">b += a</span>". Leo wants to test handling large integers, so he wants to make the value of either <span class="tex-font-style-tt">a</span> or <span class="tex-font-style-tt">b</span> <span class="tex-font-style-bf">strictly greater</span> than a given value $n$. What is the smallest number of operations he has to perform?</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \leq T \leq 100$)&nbsp;！ the number of test cases.</p><p>Each of the following $T$ lines describes a single test case, and contains three integers $a, b, n$ ($1 \leq a, b \leq n \leq 10^9$)&nbsp;！ initial values of <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>, and the value one of the variables has to exceed, respectively.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;！ the smallest number of operations needed. Separate answers with line breaks.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \leq T \leq 100$)&nbsp;！ the number of test cases.</p><p>Each of the following $T$ lines describes a single test case, and contains three integers $a, b, n$ ($1 \leq a, b \leq n \leq 10^9$)&nbsp;！ initial values of <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>, and the value one of the variables has to exceed, respectively.</p>

## Output

<p>For each test case print a single integer&nbsp;！ the smallest number of operations needed. Separate answers with line breaks.</p>

## Samples

```input1
2
1 2 3
5 4 100
```

```output1
2
7
```




## Note

<p>In the first case we cannot make a variable exceed $3$ in one operation. One way of achieving this in two operations is to perform "<span class="tex-font-style-tt">b += a</span>" twice.</p>
