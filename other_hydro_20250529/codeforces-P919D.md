## Description

<div><p>You are given a graph with $n$ nodes and $m$ <span class="tex-font-style-bf">directed</span> edges. One lowercase letter is assigned to each node. We define a path's value as the number of the most frequently occurring letter. For example, if letters on a path are "<span class="tex-font-style-tt">abaca</span>", then the value of that path is $3$. Your task is find a path whose value is the largest.</p></div><div class="input-specification"><p>The first line contains two positive integers $n, m$ ($1 \leq n, m \leq 300\,000$), denoting that the graph has $n$ nodes and $m$ directed edges.</p><p>The second line contains a string $s$ with only lowercase English letters. The $i$-th character is the letter assigned to the $i$-th node.</p><p>Then $m$ lines follow. Each line contains two integers $x, y$ ($1 \leq x, y \leq n$), describing a directed edge from $x$ to $y$. Note that $x$ can be equal to $y$ and there can be multiple edges between $x$ and $y$. Also the graph can be not connected.</p></div><div class="output-specification"><p>Output a single line with a single integer denoting the largest value. If the value can be arbitrarily large, output <span class="tex-font-style-tt">-1</span> instead.</p></div>

## Input

<p>The first line contains two positive integers $n, m$ ($1 \leq n, m \leq 300\,000$), denoting that the graph has $n$ nodes and $m$ directed edges.</p><p>The second line contains a string $s$ with only lowercase English letters. The $i$-th character is the letter assigned to the $i$-th node.</p><p>Then $m$ lines follow. Each line contains two integers $x, y$ ($1 \leq x, y \leq n$), describing a directed edge from $x$ to $y$. Note that $x$ can be equal to $y$ and there can be multiple edges between $x$ and $y$. Also the graph can be not connected.</p>

## Output

<p>Output a single line with a single integer denoting the largest value. If the value can be arbitrarily large, output <span class="tex-font-style-tt">-1</span> instead.</p>

## Samples

```input1
5 4
abaca
1 2
1 3
3 4
4 5

```

```output1
3

```






```input2
6 6
xzyabc
1 2
3 1
2 3
5 4
4 3
6 4

```

```output2
-1

```






```input3
10 14
xzyzyzyzqx
1 2
2 4
3 5
4 5
2 6
6 8
6 5
2 10
3 9
10 9
4 6
1 10
2 8
3 7

```

```output3
4

```




## Note

<p>In the first sample, the path with largest value is $1 \to 3 \to 4 \to 5$. The value is $3$ because the letter '<span class="tex-font-style-tt">a</span>' appears $3$ times.</p>
