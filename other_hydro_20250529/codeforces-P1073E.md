## Description

<div><p>You are given two integers $l$ and $r$ ($l \le r$). Your task is to calculate the sum of numbers from $l$ to $r$ (including $l$ and $r$) such that each number contains <span class="tex-font-style-bf">at most</span> $k$ different digits, and print this sum modulo $998244353$.</p><p>For example, if $k = 1$ then you have to calculate all numbers from $l$ to $r$ such that each number is formed using only one digit. For $l = 10, r = 50$ the answer is $11 + 22 + 33 + 44 = 110$.</p></div><div class="input-specification"><p>The only line of the input contains three integers $l$, $r$ and $k$ ($1 \le l \le r &lt; 10^{18}, 1 \le k \le 10$) �� the borders of the segment and the maximum number of different digits.</p></div><div class="output-specification"><p>Print one integer �� the sum of numbers from $l$ to $r$ such that each number contains at most $k$ different digits, modulo $998244353$.</p></div>

## Input

<p>The only line of the input contains three integers $l$, $r$ and $k$ ($1 \le l \le r &lt; 10^{18}, 1 \le k \le 10$) �� the borders of the segment and the maximum number of different digits.</p>

## Output

<p>Print one integer �� the sum of numbers from $l$ to $r$ such that each number contains at most $k$ different digits, modulo $998244353$.</p>

## Samples

```input1
10 50 2

```

```output1
1230

```






```input2
1 2345 10

```

```output2
2750685

```






```input3
101 154 2

```

```output3
2189

```




## Note

<p>For the first example the answer is just the sum of numbers from $l$ to $r$ which equals to $\frac{50 \cdot 51}{2} - \frac{9 \cdot 10}{2} = 1230$. This example also explained in the problem statement but for $k = 1$.</p><p>For the second example the answer is just the sum of numbers from $l$ to $r$ which equals to $\frac{2345 \cdot 2346}{2} = 2750685$.</p><p>For the third example the answer is $101 + 110 + 111 + 112 + 113 + 114 + 115 + 116 + 117 + 118 + 119 + 121 + 122 + 131 + 133 + 141 + 144 + 151 = 2189$.</p>
