## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$ of integer numbers.</p><p>Your task is to divide the array into the maximum number of segments in such a way that:</p><ul> <li> each element is contained in <span class="tex-font-style-bf">exactly one</span> segment; </li><li> each segment contains at least one element; </li><li> there doesn't exist a non-empty subset of segments such that bitwise XOR of the numbers from them is equal to $0$. </li></ul><p>Print the maximum number of segments the array can be divided into. Print <span class="tex-font-style-tt">-1</span> if no suitable division exists.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) �� the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print the maximum number of segments the array can be divided into while following the given constraints. Print <span class="tex-font-style-tt">-1</span> if no suitable division exists.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) �� the size of the array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p>

## Output

<p>Print the maximum number of segments the array can be divided into while following the given constraints. Print <span class="tex-font-style-tt">-1</span> if no suitable division exists.</p>

## Samples

```input1
4
5 5 7 2
```

```output1
2
```






```input2
3
1 2 3
```

```output2
-1
```






```input3
3
3 1 10
```

```output3
3
```




## Note

<p>In the first example $2$ is the maximum number. If you divide the array into $\{[5], [5, 7, 2]\}$, the XOR value of the subset of only the second segment is $5 \oplus 7 \oplus 2 = 0$. $\{[5, 5], [7, 2]\}$ has the value of the subset of only the first segment being $5 \oplus 5 = 0$. However, $\{[5, 5, 7], [2]\}$ will lead to subsets $\{[5, 5, 7]\}$ of XOR $7$, $\{[2]\}$ of XOR $2$ and $\{[5, 5, 7], [2]\}$ of XOR $5 \oplus 5 \oplus 7 \oplus 2 = 5$.</p><p>Let's take a look at some division on $3$ segments �� $\{[5], [5, 7], [2]\}$. It will produce subsets:</p><ul> <li> $\{[5]\}$, XOR $5$; </li><li> $\{[5, 7]\}$, XOR $2$; </li><li> $\{[5], [5, 7]\}$, XOR $7$; </li><li> $\{[2]\}$, XOR $2$; </li><li> $\{[5], [2]\}$, XOR $7$; </li><li> $\{[5, 7], [2]\}$, XOR $0$; </li><li> $\{[5], [5, 7], [2]\}$, XOR $5$; </li></ul><p>As you can see, subset $\{[5, 7], [2]\}$ has its XOR equal to $0$, which is unacceptable. You can check that for other divisions of size $3$ or $4$, non-empty subset with $0$ XOR always exists.</p><p>The second example has no suitable divisions.</p><p>The third example array can be divided into $\{[3], [1], [10]\}$. No subset of these segments has its XOR equal to $0$.</p>
