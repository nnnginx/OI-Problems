## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">As a tester, when my solution has a different output from the example during testing, I suspect the author first.</span></div><div class="epigraph-source">！ Chris, <a href="https://mirror.codeforces.com/blog/entry/133116?#comment-1190579"><span class="tex-font-style-it">a comment</span></a></div></div><p><span class="tex-font-style-it">Although Iris occasionally sets a problem where the solution is possibly wrong, she still insists on creating problems with her imagination; after all, everyone has always been on the road with their stubbornness... And like ever before, Iris has set a problem to which she gave a wrong solution, but Chris is always supposed to save it! You are going to play the role of Chris now:</span></p><ul> <li> Chris is given two arrays $a$ and $b$, both consisting of $n$ integers. </li><li> Iris is interested in the <span class="tex-font-style-bf">largest</span> possible value of $P = \prod\limits_{i=1}^n \min(a_i, b_i)$ after an arbitrary rearrangement of $b$. Note that she only wants to know the maximum value of $P$, and <span class="tex-font-style-bf">no</span> actual rearrangement is performed on $b$. </li><li> There will be $q$ modifications. Each modification can be denoted by two integers $o$ and $x$ ($o$ is either $1$ or $2$, $1 \leq x \leq n$). If $o = 1$, then Iris will increase $a_x$ by $1$; otherwise, she will increase $b_x$ by $1$. </li><li> Iris asks Chris the maximum value of $P$ for $q + 1$ times: once before any modification, then after every modification. </li><li> Since $P$ might be huge, Chris only needs to calculate it modulo $998\,244\,353$. </li></ul><p>Chris soon worked out this problem, but he was so tired that he fell asleep. Besides saying thanks to Chris, now it is your turn to write a program to calculate the answers for given input data.</p><p><span class="tex-font-style-bf">Note</span>: since the input and output are large, you may need to optimize them for this problem.</p><p>For example, in C++, it is enough to use the following lines at the start of the <span class="tex-font-style-it">main()</span> function:</p><pre class="lstlisting"><code class="prettyprint">int main() {<br>    std::ios::sync_with_stdio(false);<br>    std::cin.tie(nullptr); std::cout.tie(nullptr);<br>}<br></code></pre></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n \leq 2\cdot 10^5$, $1 \leq q \leq 2\cdot 10^5$)&nbsp;！ the length of the array and the number of operations.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 5\cdot 10^8$)&nbsp;！ the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 5\cdot 10^8$)&nbsp;！ the array $b$.</p><p>Then $q$ lines follow, each line contains two integers $o$ and $x$ ($o \in \{1, 2\}$, $1 \leq x \leq n$), representing an operation.</p><p>It's guaranteed that the sum of $n$ and the sum of $q$ over all test cases does not exceed $4\cdot 10^5$, respectively.</p></div><div class="output-specification"><p>For each test case, output $q + 1$ integers in a line, representing the answers that Chris will calculate, modulo $998\,244\,353$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains two integers $n$ and $q$ ($1 \leq n \leq 2\cdot 10^5$, $1 \leq q \leq 2\cdot 10^5$)&nbsp;！ the length of the array and the number of operations.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 5\cdot 10^8$)&nbsp;！ the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 5\cdot 10^8$)&nbsp;！ the array $b$.</p><p>Then $q$ lines follow, each line contains two integers $o$ and $x$ ($o \in \{1, 2\}$, $1 \leq x \leq n$), representing an operation.</p><p>It's guaranteed that the sum of $n$ and the sum of $q$ over all test cases does not exceed $4\cdot 10^5$, respectively.</p>

## Output

<p>For each test case, output $q + 1$ integers in a line, representing the answers that Chris will calculate, modulo $998\,244\,353$.</p>





```input1|2,3,4,5,6,7,8,20,21,22,23,24,25,26,27,28,29,30
4
3 4
1 1 2
3 2 1
1 3
2 3
1 1
2 1
6 8
1 4 2 7 3 5
7 6 5 6 3 3
2 5
1 6
1 5
1 5
1 5
2 3
2 3
1 6
13 8
7 7 6 6 5 5 5 2 2 3 4 5 1
1 4 1 9 6 6 9 1 5 1 3 8 4
2 2
2 11
2 4
2 4
1 7
1 1
2 12
1 5
5 3
10000000 20000000 30000000 40000000 50000000
10000000 20000000 30000000 40000000 50000000
1 1
2 2
2 1
```




```output1
2 3 3 6 6
840 840 1008 1344 1680 2016 2016 2016 2352
2116800 2646000 3528000 3528000 3528000 4233600 4838400 4838400 4838400
205272023 205272023 205272023 264129429
```



## Note

<p>In the first test case: </p><ul> <li> Before the modifications, Chris can rearrange $b$ to $[1, 2, 3]$ so that $P = \prod\limits_{i=1}^n \min(a_i, b_i) = 1 \cdot 1 \cdot 2 = 2$. We can prove that this is the maximum possible value. For example, if Chris rearranges $b = [2, 3, 1]$, $P$ will be equal $1 \cdot 1 \cdot 1 = 1 &lt; 2$, which is not optimal. </li><li> After the first modification, Chris can rearrange $b$ to $[1, 2, 3]$ so that $P = 1 \cdot 1 \cdot 3 = 3$, which is maximized. </li><li> After the second modification, Chris can rearrange $b$ to $[2, 2, 3]$ so that $P = 1 \cdot 1 \cdot 3 = 3$, which is maximized. </li><li> After the third modification, Chris can rearrange $b$ to $[2, 2, 3]$ so that $P = 6$, which is maximized. </li><li> After the fourth modification, Chris can rearrange $b$ to $[2, 2, 4]$ so that $P = 6$, which is maximized. </li></ul>
