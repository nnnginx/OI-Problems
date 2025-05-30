## Description

<div><p><span class="tex-font-style-it">The tycoon of a winery empire in Mondstadt, unmatched in every possible way. A thinker in the Knights of Favonius with an exotic appearance.</span></p><p>This time, the brothers are dealing with a strange piece of wood marked with their names. This plank of wood can be represented as a string of $n$ characters. Each character is either a <span class="tex-font-style-tt">'D'</span> or a <span class="tex-font-style-tt">'K'</span>. You want to make some number of cuts (possibly $0$) on this string, partitioning it into several contiguous pieces, each with length at least $1$. Both brothers act with dignity, so they want to split the wood as evenly as possible. They want to know the maximum number of pieces you can split the wood into such that the ratios of the number of occurrences of <span class="tex-font-style-tt">'D'</span> to the number of occurrences of <span class="tex-font-style-tt">'K'</span> in each chunk are the same.</p><p>Kaeya, the curious thinker, is interested in the solution for multiple scenarios. He wants to know the answer for every <span class="tex-font-style-bf">prefix</span> of the given string. Help him to solve this problem!</p><p>For a string we define a ratio as $a:b$ where <span class="tex-font-style-tt">'D'</span> appears in it $a$ times, and <span class="tex-font-style-tt">'K'</span> appears $b$ times. Note that $a$ or $b$ can equal $0$, but not both. Ratios $a:b$ and $c:d$ are considered equal if and only if $a\cdot d = b\cdot c$. </p><p>For example, for the string <span class="tex-font-style-tt">'DDD'</span> the ratio will be $3:0$, for <span class="tex-font-style-tt">'DKD'</span> ！ $2:1$, for <span class="tex-font-style-tt">'DKK'</span> ！ $1:2$, and for <span class="tex-font-style-tt">'KKKKDD'</span> ！ $2:4$. Note that the ratios of the latter two strings are equal to each other, but they are not equal to the ratios of the first two strings.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 5 \cdot 10^5$)&nbsp;！ the length of the wood.</p><p>The second line of each test case contains a string $s$ of length $n$. Every character of $s$ will be either <span class="tex-font-style-tt">'D'</span> or <span class="tex-font-style-tt">'K'</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ space separated integers. The $i$-th of these numbers should equal the answer for the prefix $s_{1},s_{2},\dots,s_{i}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 5 \cdot 10^5$)&nbsp;！ the length of the wood.</p><p>The second line of each test case contains a string $s$ of length $n$. Every character of $s$ will be either <span class="tex-font-style-tt">'D'</span> or <span class="tex-font-style-tt">'K'</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, output $n$ space separated integers. The $i$-th of these numbers should equal the answer for the prefix $s_{1},s_{2},\dots,s_{i}$.</p>

## Samples

```input1
5
3
DDK
6
DDDDDD
4
DKDK
1
D
9
DKDKDDDDK
```

```output1
1 2 1 
1 2 3 4 5 6 
1 1 1 2 
1 
1 1 1 2 1 2 1 1 3
```




## Note

<p>For the first test case, there is no way to partition <span class="tex-font-style-tt">'D'</span> or <span class="tex-font-style-tt">'DDK'</span> into more than one block with equal ratios of numbers of <span class="tex-font-style-tt">'D'</span> and <span class="tex-font-style-tt">'K'</span>, while you can split <span class="tex-font-style-tt">'DD'</span> into <span class="tex-font-style-tt">'D'</span> and <span class="tex-font-style-tt">'D'</span>.</p><p>For the second test case, you can split each prefix of length $i$ into $i$ blocks <span class="tex-font-style-tt">'D'</span>.</p>
