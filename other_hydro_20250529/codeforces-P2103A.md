## Description

<div><p> </p><p>You are given an array of integers $a_1, a_2, \ldots, a_n$. An array $x_1, x_2, \ldots, x_m$ is <span class="tex-font-style-it">beautiful</span> if there exists an array $y_1, y_2, \ldots, y_m$ such that the elements of $y$ are distinct (in other words, $y_i\neq y_j$ for all $1 \le i &lt; j \le m$), and the product of $x_i$ and $y_i$ is the same for all $1 \le i \le m$ (in other words, $x_i\cdot y_i = x_j\cdot y_j$ for all $1 \le i &lt; j \le m$).</p><p>Your task is to determine the maximum size of a subsequence$^{\text{∗}}$ of array $a$ that is beautiful.</p><div class="statement-footnote"><p>$^{\text{∗}}$A sequence $b$ is a subsequence of a sequence $a$ if $b$ can be obtained from $a$ by the deletion of several (possibly, zero or all) element from arbitrary positions. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.  </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of array $a$.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p></div><div class="output-specification"><p>For each test case, output the maximum size of a subsequence of array $a$ that is beautiful.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.  </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;— the elements of array $a$.</p><p>Note that there are <span class="tex-font-style-bf">no</span> constraints on the sum of $n$ over all test cases.</p>

## Output

<p>For each test case, output the maximum size of a subsequence of array $a$ that is beautiful.</p>





```input1|2,3,6,7
3
3
1 2 3
5
3 1 4 1 5
1
1
```




```output1
3
4
1
```



## Note

<p>In the first test case, the entire array $a = [1, 2, 3]$ is already beautiful. A possible array $y$ is $[6, 3, 2]$, which is valid since the elements of $y$ are distinct, and $1\cdot 6 = 2\cdot 3 = 3\cdot 2$.</p><p>In the second test case, the subsequence $[3, 1, 4, 5]$ is beautiful. A possible array $y$ is $[20, 60, 15, 12]$. It can be proven that the entire array $a = [3, 1, 4, 1, 5]$ is not beautiful, so the maximum size of a subsequence of array $a$ that is beautiful is $4$.</p>
