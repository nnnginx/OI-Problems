## Description

<div><p>The new generation external memory contains an array of integers $a[1 \ldots n] = [a_1, a_2, \ldots, a_n]$.</p><p>This type of memory does not support changing the value of an arbitrary element. Instead, it allows you to cut out any segment of the given array, <span class="tex-font-style-it">cyclically shift</span> (rotate) it by any offset and insert it back into the same place.</p><p>Technically, each cyclic shift consists of two consecutive actions: </p><ol> <li> You may select arbitrary indices $l$ and $r$ ($1 \le l &lt; r \le n$) as the boundaries of the segment. </li><li> Then you replace the segment $a[l \ldots r]$ with it's <span class="tex-font-style-it">cyclic shift</span> to the <span class="tex-font-style-bf">left</span> by an arbitrary offset $d$. The concept of a <span class="tex-font-style-it">cyclic shift</span> can be also explained by following relations: the sequence $[1, 4, 1, 3]$ is a cyclic shift of the sequence $[3, 1, 4, 1]$ to the left by the offset $1$ and the sequence $[4, 1, 3, 1]$ is a cyclic shift of the sequence $[3, 1, 4, 1]$ to the left by the offset $2$. </li></ol><p>For example, if $a = [1, \color{blue}{3, 2, 8}, 5]$, then choosing $l = 2$, $r = 4$ and $d = 2$ yields a segment $a[2 \ldots 4] = [3, 2, 8]$. This segment is then shifted by the offset $d = 2$ to the <span class="tex-font-style-bf">left</span>, and you get a segment $[8, 3, 2]$ which then takes the place of of the original elements of the segment. In the end you get $a = [1, \color{blue}{8, 3, 2}, 5]$.</p><p>Sort the given array $a$ using no more than $n$ cyclic shifts of any of its segments. Note that you don't need to minimize the number of cyclic shifts. Any method that requires $n$ or less cyclic shifts will be accepted.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The next $2t$ lines contain the descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($2 \leq n \leq 50$)&nbsp;！ the length of the array. The second line consists of space-separated elements of the array $a_i$ ($-10^9 \leq a_i \leq 10^9$). Elements of array $a$ may repeat and don't have to be unique.</p></div><div class="output-specification"><p>Print $t$ answers to all input test cases. </p><p>The first line of the answer of each test case should contain an integer $k$ ($0 \le k \le n$)&nbsp;！ the number of actions to sort the array. The next $k$ lines should contain descriptions of the actions formatted as "$l$<span class="tex-font-style-tt">&nbsp;</span>$r$<span class="tex-font-style-tt">&nbsp;</span>$d$" (without quotes) where $l$ and $r$ ($1 \le l &lt; r \le n$) are the boundaries of the segment being shifted, while $d$ ($1 \le d \le r - l$) is the offset value. Please remember that only the cyclic shifts <span class="tex-font-style-bf">to the left</span> are considered so the chosen segment will be shifted by the offset $d$ to the <span class="tex-font-style-it">to the left</span>.</p><p>Note that you are not required to find the minimum number of cyclic shifts needed for sorting. Any sorting method where the number of shifts does not exceed $n$ will be accepted.</p><p>If the given array $a$ is already sorted, one of the possible answers is $k = 0$ and an empty sequence of cyclic shifts.</p><p>If there are several possible answers, you may print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;！ the number of test cases.</p><p>The next $2t$ lines contain the descriptions of the test cases. </p><p>The first line of each test case description contains an integer $n$ ($2 \leq n \leq 50$)&nbsp;！ the length of the array. The second line consists of space-separated elements of the array $a_i$ ($-10^9 \leq a_i \leq 10^9$). Elements of array $a$ may repeat and don't have to be unique.</p>

## Output

<p>Print $t$ answers to all input test cases. </p><p>The first line of the answer of each test case should contain an integer $k$ ($0 \le k \le n$)&nbsp;！ the number of actions to sort the array. The next $k$ lines should contain descriptions of the actions formatted as "$l$<span class="tex-font-style-tt">&nbsp;</span>$r$<span class="tex-font-style-tt">&nbsp;</span>$d$" (without quotes) where $l$ and $r$ ($1 \le l &lt; r \le n$) are the boundaries of the segment being shifted, while $d$ ($1 \le d \le r - l$) is the offset value. Please remember that only the cyclic shifts <span class="tex-font-style-bf">to the left</span> are considered so the chosen segment will be shifted by the offset $d$ to the <span class="tex-font-style-it">to the left</span>.</p><p>Note that you are not required to find the minimum number of cyclic shifts needed for sorting. Any sorting method where the number of shifts does not exceed $n$ will be accepted.</p><p>If the given array $a$ is already sorted, one of the possible answers is $k = 0$ and an empty sequence of cyclic shifts.</p><p>If there are several possible answers, you may print any of them.</p>

## Samples

```input1
4
2
2 1
3
1 2 1
4
2 4 1 3
5
2 5 1 4 3
```

```output1
1
1 2 1
1
1 3 2
3
2 4 1
2 3 1
1 3 2
4
2 4 2
1 5 3
1 2 1
1 3 1
```




## Note

<p>Explanation of the fourth data set in the example: </p><ol> <li> The segment $a[2 \ldots 4]$ is selected and is shifted to the left by $2$: $[2, \color{blue}{5, 1, 4}, 3] \longrightarrow [2, \color{blue}{4, 5, 1}, 3]$ </li><li> The segment $a[1 \ldots 5]$ is then selected and is shifted to the left by $3$: $[\color{blue}{2, 4, 5, 1, 3}] \longrightarrow [\color{blue}{1, 3, 2, 4, 5}]$ </li><li> After that the segment $a[1 \ldots 2]$ is selected and is shifted to the left by $1$: $[\color{blue}{1, 3}, 2, 4, 5] \longrightarrow [\color{blue}{3, 1}, 2, 4, 5]$ </li><li> And in the end the segment $a[1 \ldots 3]$ is selected and is shifted to the left by $1$: $[\color{blue}{3, 1, 2}, 4, 5] \longrightarrow [\color{blue}{1, 2, 3}, 4, 5]$ </li></ol>
