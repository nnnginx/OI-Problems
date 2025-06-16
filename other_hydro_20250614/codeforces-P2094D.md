## Description

<div><p>You have two drums in front of you: a left drum and a right drum. A hit on the left can be recorded as "<span class="tex-font-style-tt">L</span>", and a hit on the right as "<span class="tex-font-style-tt">R</span>".</p><p>The strange forces that rule this world are fickle: sometimes, a blow sounds once, and sometimes it sounds twice. Therefore, a hit on the left drum could have sounded as either "<span class="tex-font-style-tt">L</span>" or "<span class="tex-font-style-tt">LL</span>", and a hit on the right drum could have sounded as either "<span class="tex-font-style-tt">R</span>" or "<span class="tex-font-style-tt">RR</span>".</p><p>The sequence of hits made is recorded in the string $p$, and the sounds heard are in the string $s$. Given $p$ and $s$, determine whether it is true that the string $s$ could have been the result of the hits from the string $p$.</p><p>For example, if $p=$"<span class="tex-font-style-tt">LR</span>", then the result of the hits could be any of the strings "<span class="tex-font-style-tt">LR</span>", "<span class="tex-font-style-tt">LRR</span>", "<span class="tex-font-style-tt">LLR</span>", and "<span class="tex-font-style-tt">LLRR</span>", but the strings "<span class="tex-font-style-tt">LLLR</span>" or "<span class="tex-font-style-tt">LRL</span>" cannot.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¨C the number of independent test cases.</p><p>The first line of each test case contains the string $p$ ($1 \le |p| \le 2 \cdot 10^5$) consisting only of the characters "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">L</span>", where $|p|$ denotes the length of the string $p$.</p><p>The second line of each test case contains the string $s$ ($1 \le |p| \le |s| \le 2 \cdot 10^5$) consisting only of the characters "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">L</span>".</p><p>It is guaranteed that the sum of $|s|$ does not exceed $2\cdot 10^5$ across all test cases.</p></div><div class="output-specification"><p>For each set of input data, output "<span class="tex-font-style-tt">YES</span>" if $s$ can be the heard sound, and "<span class="tex-font-style-tt">NO</span>" otherwise. You may output in any case.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;¨C the number of independent test cases.</p><p>The first line of each test case contains the string $p$ ($1 \le |p| \le 2 \cdot 10^5$) consisting only of the characters "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">L</span>", where $|p|$ denotes the length of the string $p$.</p><p>The second line of each test case contains the string $s$ ($1 \le |p| \le |s| \le 2 \cdot 10^5$) consisting only of the characters "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">L</span>".</p><p>It is guaranteed that the sum of $|s|$ does not exceed $2\cdot 10^5$ across all test cases.</p>

## Output

<p>For each set of input data, output "<span class="tex-font-style-tt">YES</span>" if $s$ can be the heard sound, and "<span class="tex-font-style-tt">NO</span>" otherwise. You may output in any case.</p>





```input1|2,3,6,7,10,11
5
R
RR
LRLR
LRLR
LR
LLLR
LLLLLRL
LLLLRRLL
LLRLRLRRL
LLLRLRRLLRRRL
```




```output1
YES
YES
NO
NO
YES
```


