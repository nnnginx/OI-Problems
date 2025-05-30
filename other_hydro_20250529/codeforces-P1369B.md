## Description

<div><p><span class="tex-font-style-it">Lee was cleaning his house for the party when he found a messy string under the carpets. Now he'd like to make it clean accurately and in a stylish way...</span></p><p>The string $s$ he found is a binary string of length $n$ (i. e. string consists only of <span class="tex-font-style-tt">0</span>-s and <span class="tex-font-style-tt">1</span>-s).</p><p>In one move he can choose two consecutive characters $s_i$ and $s_{i+1}$, and if $s_i$ is <span class="tex-font-style-tt">1</span> and $s_{i + 1}$ is <span class="tex-font-style-tt">0</span>, he can erase <span class="tex-font-style-bf">exactly one of them</span> (he can choose which one to erase but he can't erase both characters simultaneously). The string shrinks after erasing.</p><p>Lee can make an arbitrary number of moves (possibly zero) and he'd like to make the string $s$ as <span class="tex-font-style-it">clean</span> as possible. He thinks for two different strings $x$ and $y$, the <span class="tex-font-style-bf">shorter</span> string is cleaner, and if they are the same length, then the <span class="tex-font-style-it">lexicographically smaller</span> string is cleaner.</p><p>Now you should answer $t$ test cases: for the $i$-th test case, print the cleanest possible string that Lee can get by doing some number of moves.</p><p>Small reminder: if we have two strings $x$ and $y$ of the same length then $x$ is lexicographically smaller than $y$ if there is a position $i$ such that $x_1 = y_1$, $x_2 = y_2$,..., $x_{i - 1} = y_{i - 1}$ and $x_i &lt; y_i$.</p></div><div class="input-specification"><p>The first line contains the integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. </p><p>Next $2t$ lines contain test cases&nbsp;！ one per two lines.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the string $s$.</p><p>The second line contains the binary string $s$. The string $s$ is a string of length $n$ which consists only of zeroes and ones.</p><p>It's guaranteed that sum of $n$ over test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>Print $t$ answers&nbsp;！ one per test case.</p><p>The answer to the $i$-th test case is the cleanest string Lee can get after doing some number of moves (possibly zero).</p></div>

## Input

<p>The first line contains the integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. </p><p>Next $2t$ lines contain test cases&nbsp;！ one per two lines.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of the string $s$.</p><p>The second line contains the binary string $s$. The string $s$ is a string of length $n$ which consists only of zeroes and ones.</p><p>It's guaranteed that sum of $n$ over test cases doesn't exceed $10^5$.</p>

## Output

<p>Print $t$ answers&nbsp;！ one per test case.</p><p>The answer to the $i$-th test case is the cleanest string Lee can get after doing some number of moves (possibly zero).</p>

## Samples

```input1
5
10
0001111111
4
0101
8
11001101
10
1110000000
1
1
```

```output1
0001111111
001
01
0
1
```




## Note

<p>In the first test case, Lee can't perform any moves.</p><p>In the second test case, Lee should erase $s_2$.</p><p>In the third test case, Lee can make moves, for example, in the following order: 11001<span class="tex-font-style-underline">10</span>1&nbsp;$\rightarrow$ 1<span class="tex-font-style-underline">10</span>0101&nbsp;$\rightarrow$ 1<span class="tex-font-style-underline">10</span>101&nbsp;$\rightarrow$ <span class="tex-font-style-underline">10</span>101&nbsp;$\rightarrow$ 1<span class="tex-font-style-underline">10</span>1&nbsp;$\rightarrow$ <span class="tex-font-style-underline">10</span>1&nbsp;$\rightarrow$ 01.</p>
