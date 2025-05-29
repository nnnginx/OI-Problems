## Description

<div><p>You are given $n$ integers, each integer is from $1$ to $n$, all of them are pairwise distinct. You have to paint them red and blue (each integer should have exactly one color).</p><p>The cost of painting is the number of pairs $(x, y)$ such that $y \bmod x = 0$, $y$ is red and $x$ is blue.</p><p>For each $k \in [1, n]$, calculate the maximum cost of painting if exactly $k$ integers should have a red color.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 10^5$).</p></div><div class="output-specification"><p>For each $k \in [1,n]$ print one integer ¡ª the maximum cost of painting, if exactly $k$ integers should be red.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 10^5$).</p>

## Output

<p>For each $k \in [1,n]$ print one integer ¡ª the maximum cost of painting, if exactly $k$ integers should be red.</p>

## Samples

```input1
6
```

```output1
3 5 6 6 5 0
```






```input2
2
```

```output2
1 0
```






```input3
11
```

```output3
3 6 9 11 12 13 14 14 13 10 0
```



