## Description

<div><p>  </p><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">You are the beginning of the letter, the development of a poem, and the end of a fairy tale.</span></div><div class="epigraph-source">— ilem, <a href="https://www.bilibili.com/video/BV1Jb411U7u2/"><span class="tex-font-style-it">Pinky Promise</span></a></div></div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that in this version, you need to compute the minimum length of the arrays. You can hack only if you solved all versions of this problem.</span> </p><p>Iris treasures an integer array $a_1, a_2, \ldots, a_n$. She knows this array has an interesting property: the maximum absolute value of all elements is less than or equal to the sum of all elements, that is, $\max(\lvert a_i\rvert) \leq \sum a_i$.</p><p>Iris defines the <span class="tex-font-style-it">boredom</span> of an array as its maximum subarray$^{\text{∗}}$ sum. </p><p>Iris's birthday is coming, and Victor is going to send her another array $b_1, b_2, \ldots, b_m$ as a gift. For some seemingly obvious reasons, he decides the array $b_1, b_2, \ldots, b_m$ should have the following properties.</p><ul> <li> $a_1, a_2, \ldots, a_n$ should be a subsequence$^{\text{†}}$ of $b_1, b_2, \ldots, b_m$. </li><li> The two arrays have the same sum. That is, $\sum\limits_{i=1}^n a_i = \sum\limits_{i=1}^m b_i$. </li><li> The <span class="tex-font-style-it">boredom</span> of $b_1, b_2, \ldots, b_m$ is the smallest possible. </li><li> Among the arrays with the smallest boredom, the length of the array $b$ (i.e., $m$) is the smallest possible. And in this case, Iris will understand his regard as soon as possible! </li></ul><p>Even constrained as above, there are still too many possible gifts. So Victor asks you to <span class="tex-font-style-bf">compute the value of $\boldsymbol{m}$</span> of any array $b_1, b_2, \ldots, b_m$ satisfying all the conditions above. He promises you: if you help him successfully, he will share a bit of Iris's birthday cake with you.</p><p><span class="tex-font-style-bf">Note</span>: since the input is large, you may need to optimize it for this problem.</p><p>For example, in C++, it is enough to use the following lines at the start of the <span class="tex-font-style-it">main()</span> function:</p><pre class="lstlisting"><code class="prettyprint">int main() {<br>    std::ios::sync_with_stdio(false);<br>    std::cin.tie(nullptr); std::cout.tie(nullptr);<br>}<br></code></pre><div class="statement-footnote"><p>$^{\text{∗}}$An array $c$ is a subarray of an array $d$ if $c$ can be obtained from $d$ by the deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. </p><p>$^{\text{†}}$A sequence $c$ is a subsequence of a sequence $d$ if $c$ can be obtained from $d$ by the deletion of several (possibly, zero or all) element from arbitrary positions. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains an integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 3\cdot 10^6$)&nbsp;— the length of the array $a_1, a_2, \ldots, a_n$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the initial array. It is guaranteed that $\max(\lvert a_i\rvert) \leq \sum a_i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output a single line containing an integer: the length $m$ of a valid array $b$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains an integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 3\cdot 10^6$)&nbsp;— the length of the array $a_1, a_2, \ldots, a_n$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$)&nbsp;— the initial array. It is guaranteed that $\max(\lvert a_i\rvert) \leq \sum a_i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot 10^6$.</p>

## Output

<p>For each test case, output a single line containing an integer: the length $m$ of a valid array $b$.</p>





```input1|2,3,6,7
4
4
1 2 3 4
4
2 -3 2 2
10
2 -7 6 3 -1 4 2 -5 8 -4
20
4 -2 4 3 -2 1 5 2 3 6 -5 -1 -4 -2 -3 5 -3 1 -4 1
```




```output1
4
6
14
25
```



## Note

<p>In the first test case, $a=[1, 2, 3, 4]$. The only array $b$ which satisfies all the properties above is $[1, 2, 3, 4]$, so we should output $4$.</p><p>In the second test case, $a=[2, -3, 2, 2]$. The possible arrays $b$ are $[1, 2, -3, 2, -1, 2]$ and $[2, 1, -3, 2, -1, 2]$, so we should output $6$.</p>
