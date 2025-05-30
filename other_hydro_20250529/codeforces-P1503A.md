## Description

<div><p>A sequence of brackets is called balanced if one can turn it into a valid math expression by adding characters '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">1</span>'. For example, sequences '<span class="tex-font-style-tt">(())()</span>', '<span class="tex-font-style-tt">()</span>', and '<span class="tex-font-style-tt">(()(()))</span>' are balanced, while '<span class="tex-font-style-tt">)(</span>', '<span class="tex-font-style-tt">(()</span>', and '<span class="tex-font-style-tt">(()))(</span>' are not.</p><p>You are given a binary string $s$ of length $n$. Construct two balanced bracket sequences $a$ and $b$ of length $n$ such that for all $1\le i\le n$: </p><ul> <li> if $s_i=1$, then $a_i=b_i$ </li><li> if $s_i=0$, then $a_i\ne b_i$ </li></ul><p>If it is impossible, you should report about it.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 2\cdot 10^5$, $n$ is even).</p><p>The next line contains a string $s$ of length $n$, consisting of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>If such two balanced bracked sequences exist, output "<span class="tex-font-style-tt">YES</span>" on the first line, otherwise output "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", output the balanced bracket sequences $a$ and $b$ satisfying the conditions on the next two lines.</p><p>If there are multiple solutions, you may print any.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 2\cdot 10^5$, $n$ is even).</p><p>The next line contains a string $s$ of length $n$, consisting of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>The sum of $n$ across all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>If such two balanced bracked sequences exist, output "<span class="tex-font-style-tt">YES</span>" on the first line, otherwise output "<span class="tex-font-style-tt">NO</span>". You can print each letter in any case (upper or lower).</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", output the balanced bracket sequences $a$ and $b$ satisfying the conditions on the next two lines.</p><p>If there are multiple solutions, you may print any.</p>

## Samples

```input1
3
6
101101
10
1001101101
4
1100
```

```output1
YES
()()()
((()))
YES
()()((()))
(())()()()
NO
```




## Note

<p>In the first test case, $a=$"<span class="tex-font-style-tt">()()()</span>" and $b=$"<span class="tex-font-style-tt">((()))</span>". The characters are equal in positions $1$, $3$, $4$, and $6$, which are the exact same positions where $s_i=1$.</p><p>In the second test case, $a=$"<span class="tex-font-style-tt">()()((()))</span>" and $b=$"<span class="tex-font-style-tt">(())()()()</span>". The characters are equal in positions $1$, $4$, $5$, $7$, $8$, $10$, which are the exact same positions where $s_i=1$.</p><p>In the third test case, there is no solution.</p>
