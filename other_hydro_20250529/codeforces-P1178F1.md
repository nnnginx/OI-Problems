## Description

<div><p><span class="tex-font-style-bf">This is the first subtask of problem F. The only differences between this and the second subtask are the constraints on the value of $m$ and the time limit. You need to solve both subtasks in order to hack this one.</span></p><p>There are $n+1$ distinct colours in the universe, numbered $0$ through $n$. There is a strip of paper $m$ centimetres long initially painted with colour $0$. </p><p>Alice took a brush and painted the strip using the following process. For each $i$ from $1$ to $n$, <span class="tex-font-style-bf">in this order</span>, she picks two integers $0 \leq a_i &lt; b_i \leq m$, such that the segment $[a_i, b_i]$ is currently painted with a <span class="tex-font-style-bf">single</span> colour, and repaints it with colour $i$. </p><p>Alice chose the segments in such a way that each centimetre is now painted in some colour other than $0$. Formally, the segment $[i-1, i]$ is painted with colour $c_i$ ($c_i \neq 0$). Every colour other than $0$ is visible on the strip.</p><p>Count the number of different pairs of sequences $\{a_i\}_{i=1}^n$, $\{b_i\}_{i=1}^n$ that result in this configuration. </p><p>Since this number may be large, output it modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a two integers $n$, $m$ ($1 \leq n \leq 500$, $n = m$)&nbsp;！ the number of colours excluding the colour $0$ and the length of the paper, respectively.</p><p>The second line contains $m$ space separated integers $c_1, c_2, \ldots, c_m$ ($1 \leq c_i \leq n$)&nbsp;！ the colour visible on the segment $[i-1, i]$ after the process ends. It is guaranteed that for all $j$ between $1$ and $n$ there is an index $k$ such that $c_k = j$.</p><p>Note that since in this subtask $n = m$, this means that $c$ is a permutation of integers $1$ through $n$.</p></div><div class="output-specification"><p>Output a single integer&nbsp;！ the number of ways Alice can perform the painting, modulo $998244353$.</p></div>

## Input

<p>The first line contains a two integers $n$, $m$ ($1 \leq n \leq 500$, $n = m$)&nbsp;！ the number of colours excluding the colour $0$ and the length of the paper, respectively.</p><p>The second line contains $m$ space separated integers $c_1, c_2, \ldots, c_m$ ($1 \leq c_i \leq n$)&nbsp;！ the colour visible on the segment $[i-1, i]$ after the process ends. It is guaranteed that for all $j$ between $1$ and $n$ there is an index $k$ such that $c_k = j$.</p><p>Note that since in this subtask $n = m$, this means that $c$ is a permutation of integers $1$ through $n$.</p>

## Output

<p>Output a single integer&nbsp;！ the number of ways Alice can perform the painting, modulo $998244353$.</p>

## Samples

```input1
3 3
1 2 3
```

```output1
5
```






```input2
7 7
4 5 1 6 2 3 7
```

```output2
165
```




## Note

<p>In the first example, there are $5$ ways, all depicted in the figure below. Here, $0$ is white, $1$ is red, $2$ is green and $3$ is blue.</p><p><img class="tex-graphics" src="./30239/file/AQ29XkbR.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Below is an example of a painting process that is not valid, as in the second step the segment <span class="tex-font-style-tt">1 3</span> is not single colour, and thus may not be repainted with colour $2$.</p><p><img class="tex-graphics" src="./30239/file/PU4MwSx4.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
