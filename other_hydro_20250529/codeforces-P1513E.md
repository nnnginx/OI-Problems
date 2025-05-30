## Description

<div><p>An array is called beautiful if all the elements in the array are equal.</p><p>You can transform an array using the following steps any number of times: </p><ol> <li> Choose two indices $i$ and $j$ ($1 \leq i,j \leq n$), and an integer $x$ ($1 \leq x \leq a_i$). Let $i$ be the source index and $j$ be the sink index. </li><li> Decrease the $i$-th element by $x$, and increase the $j$-th element by $x$. The resulting values at $i$-th and $j$-th index are $a_i-x$ and $a_j+x$ respectively. </li><li> The cost of this operation is $x \cdot |j-i| $. </li><li> Now the $i$-th index can no longer be the sink and the $j$-th index can no longer be the source. </li></ol> The total cost of a transformation is the sum of all the costs in step $3$.<p>For example, array $[0, 2, 3, 3]$ can be transformed into a beautiful array $[2, 2, 2, 2]$ with total cost $1 \cdot |1-3| + 1 \cdot |1-4| = 5$.</p><p>An array is called balanced, if it can be transformed into a beautiful array, and the cost of such transformation is <span class="tex-font-style-bf">uniquely</span> defined. In other words, the minimum cost of transformation into a beautiful array equals the maximum cost.</p><p>You are given an array $a_1, a_2, \ldots, a_n$ of length $n$, consisting of non-negative integers. Your task is to find the number of balanced arrays which are permutations of the given array. Two arrays are considered different, if elements at some position differ. Since the answer can be large, output it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;�� the size of the array. </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Output a single integer&nbsp;�� the number of balanced permutations modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^5$)&nbsp;�� the size of the array. </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$).</p>

## Output

<p>Output a single integer&nbsp;�� the number of balanced permutations modulo $10^9+7$.</p>

## Samples

```input1
3
1 2 3
```

```output1
6
```






```input2
4
0 4 0 4
```

```output2
2
```






```input3
5
0 11 12 13 14
```

```output3
120
```




## Note

<p>In the first example, $[1, 2, 3]$ is a valid permutation as we can consider the index with value $3$ as the source and index with value $1$ as the sink. Thus, after conversion we get a beautiful array $[2, 2, 2]$, and the total cost would be $2$. We can show that this is the only transformation of this array that leads to a beautiful array. Similarly, we can check for other permutations too.</p><p>In the second example, $[0, 0, 4, 4]$ and $[4, 4, 0, 0]$ are balanced permutations.</p><p>In the third example, all permutations are balanced.</p>
