## Description

<div><p>The pink soldiers have given you a sequence $a$ consisting of $n$ positive integers.</p><p>You must repeatedly perform the following operation <span class="tex-font-style-bf">until there is only $1$ element left</span>.</p><ul> <li> Choose two <span class="tex-font-style-bf">distinct</span> indices $i$ and $j$. </li><li> Then, choose a positive integer value $x$ such that there exists a <span class="tex-font-style-bf">non-degenerate triangle</span>$^{\text{∗}}$ with side lengths $a_i$, $a_j$, and $x$. </li><li> Finally, remove two elements $a_i$ and $a_j$, and append $x$ to the end of $a$. </li></ul><p>Please find the maximum possible value of the only last element in the sequence $a$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A triangle with side lengths $a$, $b$, $c$ is non-degenerate when $a+b &gt; c$, $a+c &gt; b$, $b+c &gt; a$.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 1000$)&nbsp;— the elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum possible value of the only last element on a separate line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le 1000$)&nbsp;— the elements of the sequence $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum possible value of the only last element on a separate line.</p>





```input1|2,3,6,7
4
1
10
3
998 244 353
5
1 2 3 4 5
9
9 9 8 2 4 4 3 5 3
```




```output1
10
1593
11
39
```



## Note

<p>On the first test case, there is already only one element. The value of the only last element is $10$.</p><p>On the second test case, $a$ is initially $[998,244,353]$. The following series of operations is valid:</p><ol> <li> Erase $a_2=244$ and $a_3=353$, and append $596$ to the end of $a$. $a$ is now $[998,596]$. </li><li> Erase $a_1=998$ and $a_2=596$, and append $1593$ to the end of $a$. $a$ is now $[1593]$. </li></ol><p>It can be shown that the only last element cannot be greater than $1593$. Therefore, the answer is $1593$.</p>
