## Description

<div><p><span class="tex-font-style-bf">The only difference between the two versions is that this version asks the <span class="tex-font-style-it">minimal</span> possible answer.</span></p><p>Homer likes arrays a lot. Today he is painting an array $a_1, a_2, \dots, a_n$ with two kinds of colors, <span class="tex-font-style-bf">white</span> and <span class="tex-font-style-bf">black</span>. A painting assignment for $a_1, a_2, \dots, a_n$ is described by an array $b_1, b_2, \dots, b_n$ that $b_i$ indicates the color of $a_i$ ($0$ for white and $1$ for black).</p><p>According to a painting assignment $b_1, b_2, \dots, b_n$, the array $a$ is split into two new arrays $a^{(0)}$ and $a^{(1)}$, where $a^{(0)}$ is the sub-sequence of all white elements in $a$ and $a^{(1)}$ is the sub-sequence of all black elements in $a$. For example, if $a = [1,2,3,4,5,6]$ and $b = [0,1,0,1,0,0]$, then $a^{(0)} = [1,3,5,6]$ and $a^{(1)} = [2,4]$.</p><p>The number of segments in an array $c_1, c_2, \dots, c_k$, denoted $\mathit{seg}(c)$, is the number of elements if we merge all adjacent elements with the same value in $c$. For example, the number of segments in $[1,1,2,2,3,3,3,2]$ is $4$, because the array will become $[1,2,3,2]$ after merging adjacent elements with the same value. Especially, the number of segments in an empty array is $0$.</p><p>Homer wants to find a painting assignment $b$, according to which the number of segments in both $a^{(0)}$ and $a^{(1)}$, i.e. $\mathit{seg}(a^{(0)})+\mathit{seg}(a^{(1)})$, is as <span class="tex-font-style-bf">small</span> as possible. Find this number.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$).</p></div><div class="output-specification"><p>Output a single integer, indicating the <span class="tex-font-style-bf">minimal</span> possible total number of segments.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$).</p>

## Output

<p>Output a single integer, indicating the <span class="tex-font-style-bf">minimal</span> possible total number of segments.</p>

## Samples

```input1
6
1 2 3 1 2 2
```

```output1
4
```






```input2
7
1 2 1 2 1 2 1
```

```output2
2
```




## Note

<p>In the first example, we can choose $a^{(0)} = [1,1,2,2]$, $a^{(1)} = [2,3]$ and $\mathit{seg}(a^{(0)}) = \mathit{seg}(a^{(1)}) = 2$. So the answer is $2+2 = 4$.</p><p>In the second example, we can choose $a^{(0)} = [1,1,1,1]$, $a^{(1)} = [2,2,2]$ and $\mathit{seg}(a^{(0)}) = \mathit{seg}(a^{(1)}) = 1$. So the answer is $1+1 = 2$.</p>
