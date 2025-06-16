## Description

<div><p>There are balls of $n$ different colors; the number of balls of the $i$-th color is $a_i$.</p><p>The balls can be combined into groups. Each group should contain at most $2$ balls, and no more than $1$ ball of each color.</p><p>Consider all $2^n$ sets of colors. For a set of colors, let's denote its <span class="tex-font-style-it">value</span> as the minimum number of groups the balls of those colors can be distributed into. For example, if there are three colors with $3$, $1$ and $7$ balls respectively, they can be combined into $7$ groups (and not less than $7$), so the value of that set of colors is $7$.</p><p>Your task is to calculate the sum of <span class="tex-font-style-it">values</span> over all $2^n$ possible sets of colors. Since the answer may be too large, print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;！ the number of colors.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5000$)&nbsp;！ the number of balls of the $i$-th color.</p><p>Additional constraint on input: the total number of balls doesn't exceed $5000$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;！ the sum of values of all $2^n$ sets of colors, taken modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;！ the number of colors.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 5000$)&nbsp;！ the number of balls of the $i$-th color.</p><p>Additional constraint on input: the total number of balls doesn't exceed $5000$.</p>

## Output

<p>Print a single integer&nbsp;！ the sum of values of all $2^n$ sets of colors, taken modulo $998\,244\,353$.</p>





```input1|
3
1 1 2
```




```input2|
1
5
```




```input3|
4
1 3 3 7
```




```output1
11
```




```output2
5
```




```output3
76
```



## Note

<p>Consider the first example. There are $8$ sets of colors:</p><ul> <li> for the empty set, its value is $0$; </li><li> for the set $\{1\}$, its value is $1$; </li><li> for the set $\{2\}$, its value is $1$; </li><li> for the set $\{3\}$, its value is $2$; </li><li> for the set $\{1,2\}$, its value is $1$; </li><li> for the set $\{1,3\}$, its value is $2$; </li><li> for the set $\{2,3\}$, its value is $2$; </li><li> for the set $\{1,2,3\}$, its value is $2$. </li></ul><p>So, the sum of values over all $2^n$ sets of colors is $11$.</p>
