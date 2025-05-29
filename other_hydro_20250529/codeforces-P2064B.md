## Description

<div><p>Define the score of an arbitrary array $b$ to be the length of $b$ minus the number of distinct elements in $b$. For example: </p><ul> <li> The score of $[1, 2, 2, 4]$ is $1$, as it has length $4$ and only $3$ distinct elements ($1$, $2$, $4$). </li><li> The score of $[1, 1, 1]$ is $2$, as it has length $3$ and only $1$ distinct element ($1$). </li><li> The empty array has a score of $0$. </li></ul><p>You have an array $a$. You need to remove some <span class="tex-font-style-bf">non-empty</span> contiguous subarray from $a$ <span class="tex-font-style-bf">at most</span> once.</p><p>More formally, you can do the following <span class="tex-font-style-bf">at most</span> once: </p><ul> <li> pick two integers $l$, $r$ where $1 \le l \le r \le n$, and </li><li> delete the contiguous subarray $[a_l,\ldots,a_r]$ from $a$ (that is, replace $a$ with $[a_1,\ldots,a_{l - 1},a_{r + 1},\ldots,a_n]$). </li></ul><p>Output an operation such that the score of $a$ is <span class="tex-font-style-bf">maximum</span>; if there are multiple answers, output one that <span class="tex-font-style-bf">minimises</span> the final length of $a$ after the operation. If there are still multiple answers, you may output any of them.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, if you wish to not make a move, output $0$.</p><p>Otherwise, output two integers $l$ and $r$ ($1 \le l \le r \le n$), representing the left and right bound of the removed subarray.</p><p>The removed subarray should be chosen such that the score is maximized, and over all such answers choose any of them that minimises the final length of the array.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the array $a$.</p><p>The second line of each testcase contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1 \le a_i \le n$).</p><p>The sum of $n$ across all testcases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, if you wish to not make a move, output $0$.</p><p>Otherwise, output two integers $l$ and $r$ ($1 \le l \le r \le n$), representing the left and right bound of the removed subarray.</p><p>The removed subarray should be chosen such that the score is maximized, and over all such answers choose any of them that minimises the final length of the array.</p>





```input1|2,3,6,7
3
1
1
5
1 1 1 1 1
4
2 1 3 2
```




```output1
1 1
0
2 3
```



## Note

<p>In the first testcase, we have two options: </p><ul> <li> do nothing: the score of $[1]$ is $1-1=0$. </li><li> remove the subarray with $l=1$, $r=1$: we remove the only element, and we get an empty array with score $0$. </li></ul> Therefore, the maximum score possible is $0$. However, since we need to additionally minimise the final length of the array, we <span class="tex-font-style-bf">must</span> output the second option with $l=r=1$. Note that the first option of doing nothing is <span class="tex-font-style-bf">incorrect</span>, since it has a longer final length.<p>In the second testcase, no subarray is selected, so after which $a$ is still $[1, 1, 1, 1, 1]$. This has length $5$ and $1$ distinct element, so it has a score of $5 - 1 = 4$. This can be proven to be a shortest array which maximises the score.</p><p>In the third testcase, the subarray selected is $[2, \color{red}1, \color{red}3, 2]$, after which $a$ becomes $[2, 2]$. This has length $2$ and $1$ distinct element, so it has a score of $2 - 1 = 1$. This can be proven to be a shortest array which maximises the score.</p>
