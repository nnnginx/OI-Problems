## Description

<div><p>You are given a sequence $[a_1,\ldots,a_n]$ where each element $a_i$ is either $0$ or $1$. You can apply several (possibly zero) operations to the sequence. In each operation, you select two integers $1\le l\le r\le |a|$ (where $|a|$ is the current length of $a$) and replace $[a_l,\ldots,a_r]$ with a single element $x$, where $x$ is the majority of $[a_l,\ldots,a_r]$.</p><p>Here, the majority of a sequence consisting of $0$ and $1$ is defined as follows: suppose there are $c_0$ zeros and $c_1$ ones in the sequence, respectively. </p><ul> <li> If $c_0\ge c_1$, the majority is $0$. </li><li> If $c_0&lt;c_1$, the majority is $1$. </li></ul><p>For example, suppose $a=[1,0,0,0,1,1]$. If we select $l=1,r=2$, the resulting sequence will be $[0,0,0,1,1]$. If we select $l=4,r=6$, the resulting sequence will be $[1,0,0,1]$. </p><p>Determine if you can make $a=[1]$ with a finite number of operations.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 4\cdot 10^4$). Description of the test cases follows.</p><p>The first line of each testcase contains one integer $n$ ($1\le n\le 2\cdot 10^5$).</p><p>The second line of each testcase contains a string consisting of $0$ and $1$, describing the sequence $a$.</p><p>It's guaranteed that the sum of $n$ over all testcases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, if it's possible to make $a=[1]$, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>. You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 4\cdot 10^4$). Description of the test cases follows.</p><p>The first line of each testcase contains one integer $n$ ($1\le n\le 2\cdot 10^5$).</p><p>The second line of each testcase contains a string consisting of $0$ and $1$, describing the sequence $a$.</p><p>It's guaranteed that the sum of $n$ over all testcases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each testcase, if it's possible to make $a=[1]$, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>. You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span>, and <span class="tex-font-style-tt">YES</span> will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
5
1
0
1
1
2
01
9
100000001
9
000011000
```




```output1
No
Yes
No
Yes
No
```



## Note

<p>In the fourth testcase of the example, initially $a=[1,0,0,0,0,0,0,0,1]$. A valid sequence of operations is: </p><ol> <li> Select $l=2,r=8$ and apply the operation. $a$ becomes $[1,0,1]$. </li><li> Select $l=1,r=3$ and apply the operation. $a$ becomes $[1]$. </li></ol>
