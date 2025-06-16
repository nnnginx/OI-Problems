## Description

<div><p>One day, Zimpha casually came up with a problem. As a member of "Zimpha fan club", you decided to solve that problem.</p><p>You are given two strings $s$ and $t$ of length $n$ and $m$, respectively. Both strings only consist of lowercase English letters, <span class="tex-font-style-tt">-</span> and <span class="tex-font-style-tt">*</span>.</p><p>You need to replace all occurrences of <span class="tex-font-style-tt">*</span> and <span class="tex-font-style-tt">-</span>, observing the following rules:</p><ul> <li> For each <span class="tex-font-style-tt">-</span>, you must replace it with any lowercase English letter. </li><li> For each <span class="tex-font-style-tt">*</span>, you must replace it with a string of any (possibly, zero) length which only consists of lowercase English letters. </li></ul><p>Note that you can replace two different instances of <span class="tex-font-style-tt">-</span> with different characters. You can also replace each two different instances of <span class="tex-font-style-tt">*</span> with different strings.</p><p>Suppose $s$ and $t$ have been transformed into $s'$ and $t'$. Now you're wondering if there's a replacement that makes $s'=t'$.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^6$)&nbsp;¡ª the length of the strings $s$ and $t$, respectively.</p><p>The second line contains the string $s$ of length $n$. It is guaranteed that $s$ only consists of lowercase English letters, <span class="tex-font-style-tt">-</span> and <span class="tex-font-style-tt">*</span>.</p><p>The third line contains the string $t$ of length $m$. It is guaranteed that $t$ only consists of lowercase English letters, <span class="tex-font-style-tt">-</span> and <span class="tex-font-style-tt">*</span>.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if there is a replacement that makes $s'=t'$, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line of input contains two integers $n$ and $m$ ($1 \leq n, m \leq 2 \cdot 10^6$)&nbsp;¡ª the length of the strings $s$ and $t$, respectively.</p><p>The second line contains the string $s$ of length $n$. It is guaranteed that $s$ only consists of lowercase English letters, <span class="tex-font-style-tt">-</span> and <span class="tex-font-style-tt">*</span>.</p><p>The third line contains the string $t$ of length $m$. It is guaranteed that $t$ only consists of lowercase English letters, <span class="tex-font-style-tt">-</span> and <span class="tex-font-style-tt">*</span>.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if there is a replacement that makes $s'=t'$, and output "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">No</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive response).</p>





```input1|
10 10
justmonika
j-stsayori
```




```input2|
7 8
ttk-wxx
*tt-l-xx
```




```input3|
13 11
asoulwangziji
-soulg*z-y-
```




```input4|
7 3
abc*cba
a*c
```




```input5|
20 18
bulijiojio-dibuliduo
*li*ji-*ox*i*-du*-
```




```output1
No
```




```output2
Yes
```




```output3
No
```




```output4
No
```




```output5
Yes
```



## Note

<p>In the second test case, we can transform both strings into <span class="tex-font-style-tt">ttklwxx</span>. In $s$, <span class="tex-font-style-tt">-</span> will be replaced with <span class="tex-font-style-tt">l</span>. In $t$, <span class="tex-font-style-tt">*</span> will be replaced by the empty string with the first and second <span class="tex-font-style-tt">-</span> will be replaced with <span class="tex-font-style-tt">k</span> and <span class="tex-font-style-tt">w</span> respectively.</p><p>In the fifth test case, we can transform both strings into <span class="tex-font-style-tt">bulijiojioxdibuliduo</span>.</p>
