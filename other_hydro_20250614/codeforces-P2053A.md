## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">I would use a firework to announce, a wave to bid farewell, and a bow to say thanks: bygones are bygones; not only on the following path will I be walking leisurely and joyfully, but also the footsteps won't halt as time never leaves out flowing; for in the next year, we will meet again.</span></div><div class="epigraph-source">— Cocoly1990, <span class="tex-font-style-it"><a href="https://www.luogu.com.cn/problem/P8941">Goodbye 2022</a></span></div></div><p><span class="tex-font-style-it">In his dream, Cocoly would go on a long holiday with no worries around him. So he would try out for many new things, such as... being a carpenter. To learn it well, Cocoly decides to become an apprentice of Master, but in front of him lies a hard task waiting for him to solve.</span></p><p>Cocoly is given an array $a_1, a_2,\ldots, a_n$. Master calls a set of integers $S$ <span class="tex-font-style-it">stable</span> if and only if, for any possible $u$, $v$, and $w$ from the set $S$ (note that $u$, $v$, and $w$ do not necessarily have to be pairwise distinct), sticks of length $u$, $v$, and $w$ can form a non-degenerate triangle$^{\text{∗}}$.</p><p>Cocoly is asked to partition the array $a$ into several (possibly, $1$ or $n$) <span class="tex-font-style-bf">non-empty</span> continuous subsegments$^{\text{†}}$, such that: for each of the subsegments, the set containing all the elements in it is <span class="tex-font-style-it">stable</span>.</p><p>Master wants Cocoly to partition $a$ in <span class="tex-font-style-bf">at least two</span> different$^{\text{‡}}$ ways. You have to help him determine whether it is possible.</p><div class="statement-footnote"><p>$^{\text{∗}}$A triangle with side lengths $x$, $y$, and $z$ is called non-degenerate if and only if: </p><ul> <li> $x + y &gt; z$, </li><li> $y + z &gt; x$, and </li><li> $z + x &gt; y$. </li></ul><p>$^{\text{†}}$A sequence $b$ is a subsegment of a sequence $c$ if $b$ can be obtained from $c$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p><p>$^{\text{‡}}$Two partitions are considered different if and only if at least one of the following holds: </p><ul> <li> the numbers of continuous subsegments split in two partitions are different; </li><li> there is an integer $k$ such that the lengths of the $k$-th subsegment in two partitions are different. </li></ul></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 200$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 200$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— the elements in the array $a$.</p></div><div class="output-specification"><p>For each test case, print $\texttt{YES}$ if there are at least two ways to partition $a$, and $\texttt{NO}$ otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$, and $\texttt{YES}$ will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of the input contains a single integer $t$ ($1 \leq t \leq 200$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 200$)&nbsp;— the length of the array $a$.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \leq a_i \leq 10^5$)&nbsp;— the elements in the array $a$.</p>

## Output

<p>For each test case, print $\texttt{YES}$ if there are at least two ways to partition $a$, and $\texttt{NO}$ otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings $\texttt{yEs}$, $\texttt{yes}$, $\texttt{Yes}$, and $\texttt{YES}$ will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
5
4
2 3 5 7
4
115 9 2 28
5
8 4 1 6 2
6
1 5 4 1 4 7
2
100000 100000
```




```output1
YES
NO
NO
YES
YES
```



## Note

<p>In the first test case, here are two possible partitions:</p><ul> <li> $[2, 3], [5, 7]$, since <ul> <li> $[2, 3]$ is <span class="tex-font-style-it">stable</span> because sticks of lengths $(2, 2, 2), (2, 2, 3), (2, 3, 3), (3, 3, 3)$ respectively can all form non-degenerate triangles. </li><li> $[5, 7]$ is <span class="tex-font-style-it">stable</span> because sticks of lengths $(5, 5, 5), (5, 5, 7), (5, 7, 7), (7, 7, 7)$ respectively can all form non-degenerate triangles. </li></ul> </li><li> and $[2], [3, 5], [7]$, since <ul> <li> $[2]$ is <span class="tex-font-style-it">stable</span> because sticks of lengths $(2, 2, 2)$ respectively can form a non-degenerate triangle. </li><li> $[3, 5]$ is <span class="tex-font-style-it">stable</span> because sticks of lengths $(3, 3, 3), (3, 3, 5), (3, 5, 5), (5, 5, 5)$ respectively can all form non-degenerate triangles. </li><li> $[7]$ is <span class="tex-font-style-it">stable</span> because sticks of lengths $(7, 7, 7)$ respectively can form a non-degenerate triangle. </li></ul> </li></ul><p>Note that some other partitions also satisfy the constraints, such as $[2], [3], [5], [7]$ and $[2], [3], [5, 7]$. </p><p>In the second test case, Cocoly can only partition each element as a single subsegment, resulting in $[115], [9], [2], [28]$. Since we only have one possible partition, the answer is $\texttt{NO}$.</p><p>In the third test case, please note that the partition $[8, 4], [1], [6], [2]$ does not satisfy the constraints, because $\{8, 4\}$ is not a <span class="tex-font-style-it">stable</span> set: sticks of lengths $4$, $4$, and $8$ cannot form a non-degenerate triangle.</p>
