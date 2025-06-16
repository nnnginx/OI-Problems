## Description

<div><p>Today, Sakurako was studying arrays. An array $a$ of length $n$ is considered good if and only if:</p><ul> <li> the array $a$ is increasing, meaning $a_{i - 1} &lt; a_i$ for all $2 \le i \le n$; </li><li> the differences between adjacent elements are increasing, meaning $a_i - a_{i-1} &lt; a_{i+1} - a_i$ for all $2 \le i &lt; n$. </li></ul><p>Sakurako has come up with boundaries $l$ and $r$ and wants to construct a good array of maximum length, where $l \le a_i \le r$ for all $a_i$.</p><p>Help Sakurako find the maximum length of a good array for the given $l$ and $r$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1\le l\le r\le 10^9$).</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;！ the length of the longest good array Sakurako can form given $l$ and $r$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) &nbsp;！ the number of test cases.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1\le l\le r\le 10^9$).</p>

## Output

<p>For each test case, output a single integer &nbsp;！ the length of the longest good array Sakurako can form given $l$ and $r$.</p>





```input1|2,4,6
5
1 2
1 5
2 2
10 20
1 1000000000
```




```output1
2
3
1
5
44721
```



## Note

<p>For $l=1$ and $r=5$, one possible array could be $(1,2,5)$. It can be proven that an array of length $4$ does not exist for the given $l$ and $r$.</p><p>For $l=2$ and $r=2$, the only possible array is $(2)$.</p><p>For $l=10$ and $r=20$, the only possible array is $(10,11,13,16,20)$.</p>
