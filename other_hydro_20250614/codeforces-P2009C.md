## Description

<div><p>Freya the Frog is traveling on the 2D coordinate plane. She is currently at point $(0,0)$ and wants to go to point $(x,y)$. In one move, she chooses an integer $d$ such that $0 \leq d \leq k$ and jumps $d$ spots forward in the direction she is facing. </p><p>Initially, she is facing the positive $x$ direction. After every move, she will alternate between facing the positive $x$ direction and the positive $y$ direction (i.e., she will face the positive $y$ direction on her second move, the positive $x$ direction on her third move, and so on). </p><p>What is the minimum amount of moves she must perform to land on point $(x,y)$?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$) ¡ª the number of test cases.</p><p>Each test case contains three integers $x$, $y$, and $k$ ($0 \leq x, y \leq 10^9, 1 \leq k \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, output the number of jumps Freya needs to make on a new line.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$) ¡ª the number of test cases.</p><p>Each test case contains three integers $x$, $y$, and $k$ ($0 \leq x, y \leq 10^9, 1 \leq k \leq 10^9$).</p>

## Output

<p>For each test case, output the number of jumps Freya needs to make on a new line.</p>





```input1|2,4
3
9 11 3
0 10 8
1000000 100000 10
```




```output1
8
4
199999
```



## Note

<p>In the first sample, one optimal set of moves is if Freya jumps in the following way: ($0,0$) $\rightarrow$ ($2,0$) $\rightarrow$ ($2,2$) $\rightarrow$ ($3,2$) $\rightarrow$ ($3,5$) $\rightarrow$ ($6,5$) $\rightarrow$ ($6,8$) $\rightarrow$ ($9,8$) $\rightarrow$ ($9,11$). This takes 8 jumps.</p>
