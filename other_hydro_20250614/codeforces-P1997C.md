## Description

<div><p>Monocarp had a regular bracket sequence $s$ of length $n$ ($n$ is even). He even came up with his own way to calculate its cost.</p><p>He knows that in a regular bracket sequence (RBS), each opening bracket is paired up with the corresponding closing bracket. So he decided to calculate the <span class="tex-font-style-it">cost</span> of RBS as the sum of distances between pairs of corresponding bracket pairs.</p><p>For example, let's look at RBS <span class="tex-font-style-tt">(())()</span>. It has three pairs of brackets: </p><ul> <li> <span class="tex-font-style-tt">(__)__</span>: the distance between brackets at position $1$ and at $4$ is $4 - 1 = 3$; </li><li> <span class="tex-font-style-tt">_()___</span>: the distance is $3 - 2 = 1$; </li><li> <span class="tex-font-style-tt">____()</span>: the distance is $6 - 5 = 1$. </li></ul> So the cost of <span class="tex-font-style-tt">(())()</span> is $3 + 1 + 1 = 5$.<p>Unfortunately, due to data corruption, Monocarp lost all characters on odd positions $s_1, s_3, \dots, s_{n-1}$. Only characters on even positions ($s_2, s_4, \dots, s_{n}$) remain. For example, <span class="tex-font-style-tt">(())()</span> turned to <span class="tex-font-style-tt">_(_)_)</span>.</p><p>Monocarp wants to restore his RBS by placing brackets on the odd positions. But since the restored RBS may not be unique, he wants to choose one with <span class="tex-font-style-bf">minimum cost</span>. It's too hard to do for Monocarp alone, so can you help him?</p><p>Reminder: A <span class="tex-font-style-it">regular bracket sequence</span> is a string consisting of only brackets, such that this sequence, when inserted <span class="tex-font-style-tt">1</span>-s and <span class="tex-font-style-tt">+</span>-s, gives a valid mathematical expression. For example, <span class="tex-font-style-tt">()</span>, <span class="tex-font-style-tt">(())</span> or <span class="tex-font-style-tt">(()())()</span> are RBS, while <span class="tex-font-style-tt">)</span>, <span class="tex-font-style-tt">()(</span> or <span class="tex-font-style-tt">())(()</span> are not.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$; $n$ is even)&nbsp;！ the length of string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, where all characters on the odd positions are '<span class="tex-font-style-tt">_</span>' and all characters on the even positions are either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>'.</p><p>Additional constraints: </p><ul> <li> $s$ can be restored to at least one regular bracket sequence; </li><li> the total sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each test case, print one integer&nbsp;！ the minimum cost of the regular bracket sequence that can be obtained from $s$ by replacing '<span class="tex-font-style-tt">_</span>'-s with brackets.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5000$)&nbsp;！ the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$; $n$ is even)&nbsp;！ the length of string $s$.</p><p>The second line of each test case contains a string $s$ of length $n$, where all characters on the odd positions are '<span class="tex-font-style-tt">_</span>' and all characters on the even positions are either '<span class="tex-font-style-tt">(</span>' or '<span class="tex-font-style-tt">)</span>'.</p><p>Additional constraints: </p><ul> <li> $s$ can be restored to at least one regular bracket sequence; </li><li> the total sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul>

## Output

<p>For each test case, print one integer&nbsp;！ the minimum cost of the regular bracket sequence that can be obtained from $s$ by replacing '<span class="tex-font-style-tt">_</span>'-s with brackets.</p>





```input1|2,3,6,7
4
6
_(_)_)
2
_)
8
_)_)_)_)
8
_(_)_(_)
```




```output1
5
1
4
8
```



## Note

<p>In the first test case, it's optimal to make $s$ equal to <span class="tex-font-style-tt">(())()</span>. The cost of $s$ will be equal to $3 + 1 + 1 = 5$.</p><p>In the second test case, the only option is to make $s$ equal to <span class="tex-font-style-tt">()</span> with cost $1$.</p><p>In the third test case, the only possible RBS is <span class="tex-font-style-tt">()()()()</span> with cost $1 + 1 + 1 + 1 = 4$.</p><p>In the fourth test case, it's optimal to make $s$ equal to <span class="tex-font-style-tt">(())(())</span> with cost $3 + 1 + 3 + 1 = 8$.</p>
