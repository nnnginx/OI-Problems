## Description

<div><p>Let's define the operation of compressing a string $t$, consisting of at least $2$ digits from $1$ to $9$, as follows: </p><ul> <li> split it into an <span class="tex-font-style-bf">even</span> number of non-empty substrings&nbsp;¡ª let these substrings be $t_1, t_2, \dots, t_m$ (so, $t = t_1 + t_2 + \dots + t_m$, where $+$ is the concatenation operation); </li><li> write the string $t_2$ $t_1$ times, then the string $t_4$ $t_3$ times, and so on. </li></ul><p>For example, for a string "<span class="tex-font-style-tt">12345</span>", one could do the following: split it into ("<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">23</span>", "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">5</span>"), and write "<span class="tex-font-style-tt">235555</span>".</p><p>Let the function $f(t)$ for a string $t$ return the minimum length of the string that can be obtained as a result of that process.</p><p>You are given a string $s$, consisting of $n$ digits from $1$ to $9$, and an integer $k$. Calculate the value of the function $f$ for all contiguous substrings of $s$ of length exactly $k$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le k \le n \le 2 \cdot 10^5$).</p><p>The second line contains the string $s$ ($|s| = n$), consisting only of digits from $1$ to $9$.</p></div><div class="output-specification"><p>Output $n - k + 1$ integers&nbsp;¡ª $f(s_{1,k}), f(s_{2,k+1}), \dots, f(s_{n - k + 1, n})$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le k \le n \le 2 \cdot 10^5$).</p><p>The second line contains the string $s$ ($|s| = n$), consisting only of digits from $1$ to $9$.</p>

## Output

<p>Output $n - k + 1$ integers&nbsp;¡ª $f(s_{1,k}), f(s_{2,k+1}), \dots, f(s_{n - k + 1, n})$.</p>





```input1|
4 4
5999
```




```input2|
10 3
1111111111
```




```input3|
11 4
49998641312
```




```output1
14
```




```output2
2 2 2 2 2 2 2 2
```




```output3
12 18 17 15 12 7 7 2
```


