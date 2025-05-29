## Description

<div><p>Mocha likes arrays, so before her departure, Bazoka gave her an array $a$ consisting of $n$ positive integers as a gift.</p><p>Now Mocha wants to know whether array $a$ could become sorted in non-decreasing order after performing the following operation some (possibly, zero) times:</p><ul> <li> Split the array into two parts&nbsp;�� a prefix and a suffix, then swap these two parts. In other words, let $a=x+y$. Then, we can set $a:= y+x$. Here $+$ denotes the array concatenation operation. </li></ul><p>For example, if $a=[3,1,4,1,5]$, we can choose $x=[3,1]$ and $y=[4,1,5]$, satisfying $a=x+y$. Then, we can set $a:= y + x = [4,1,5,3,1]$. We can also choose $x=[3,1,4,1,5]$ and $y=[\,]$, satisfying $a=x+y$. Then, we can set $a := y+x = [3,1,4,1,5]$. Note that we are not allowed to choose $x=[3,1,1]$ and $y=[4,5]$, neither are we allowed to choose $x=[1,3]$ and $y=[5,1,4]$, as both these choices do not satisfy $a=x+y$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 1000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 50$)&nbsp;�� the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i \leq 10^6$)&nbsp;�� the elements of array $a$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if $a$ could become non-decreasing after performing the operation any number of times, and output "<span class="tex-font-style-tt">No</span>" if not.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 1000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 50$)&nbsp;�� the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2,\ldots,a_n$ ($1\leq a_i \leq 10^6$)&nbsp;�� the elements of array $a$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if $a$ could become non-decreasing after performing the operation any number of times, and output "<span class="tex-font-style-tt">No</span>" if not.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7
3
6
1 1 4 5 1 4
5
7 9 2 2 3
3
1 2 3
```




```output1
No
Yes
Yes
```



## Note

<p>In the first test case, it can be proven that $a$ cannot become non-decreasing after performing the operation any number of times.</p><p>In the second test case, we can perform the following operations to make $a$ sorted in non-decreasing order: </p><ul> <li> Split the array into two parts: $x=[7]$ and $y=[9,2,2,3]$, then swap these two parts. The array will become $y+x = [9,2,2,3,7]$. </li><li> Split the array into two parts: $x=[9]$ and $y=[2,2,3,7]$, then swap these two parts. The array will become $y+x=[2,2,3,7,9]$, which is non-decreasing. </li></ul>
