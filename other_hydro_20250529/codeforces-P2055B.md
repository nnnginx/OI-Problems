## Description

<div><p> </p><center><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small"><span class="tex-font-style-it">As you'd expect, Florida is home to many bizarre magical forces, and Florida Man seeks to tame them.</span></span></td></tr></tbody></table></center><p>There are $n$ different types of magical materials, numbered from $1$ to $n$. Initially, you have $a_i$ units of material $i$ for each $i$ from $1$ to $n$. You are allowed to perform the following operation:</p><ul> <li> Select a material $i$ (where $1\le i\le n$). Then, spend $1$ unit of <span class="tex-font-style-bf">every</span> other material $j$ (in other words, $j\neq i$) to gain $1$ unit of material $i$. More formally, after selecting material $i$, update array $a$ as follows: $a_i := a_i + 1$, and $a_j := a_j - 1$ for all $j$ where $j\neq i$ and $1\le j\le n$. Note that all $a_j$ must remain non-negative, i.e. you cannot spend resources you do not have. </li></ul><p>You are trying to craft an artifact using these materials. To successfully craft the artifact, you must have at least $b_i$ units of material $i$ for each $i$ from $1$ to $n$. Determine if it is possible to craft the artifact by performing the operation any number of times (including zero).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 2\cdot 10^5$)&nbsp;！ the number of types of materials.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i\le 10^9$)&nbsp;！ the amount of each material $i$ that you currently hold.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i\le 10^9$)&nbsp;！ the amount of each material $i$ needed to produce the artifact.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, print a single line containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", representing whether or not the artifact can be crafted.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 2\cdot 10^5$)&nbsp;！ the number of types of materials.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i\le 10^9$)&nbsp;！ the amount of each material $i$ that you currently hold.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($0 \le b_i\le 10^9$)&nbsp;！ the amount of each material $i$ needed to produce the artifact.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, print a single line containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", representing whether or not the artifact can be crafted.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,8,9,10
3
4
0 5 5 1
1 4 4 0
3
1 1 3
2 2 1
2
1 10
3 3
```




```output1
YES
NO
YES
```



## Note

<p>In the first test case, perform an operation on material $1$. After doing so, we will have exactly the required resources: $1$ unit of material $1$, and $4$ units each of materials $2$ and $3$.</p><p>In the second test case, it can be shown that no matter how the operations are performed, it is impossible to craft the artifact.</p><p>In the third test case, we can perform the operation on material $1$ twice. After these operations, we will have $3$ units of material $1$ and $8$ units of material $2$, which is more than enough to craft the artifact.</p>
