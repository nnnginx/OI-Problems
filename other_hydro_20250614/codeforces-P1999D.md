## Description

<div><p>Slavic has a very tough exam and needs your help in order to pass it. Here is the question he is struggling with:</p><p>There exists a string $s$, which consists of lowercase English letters and possibly zero or more "<span class="tex-font-style-tt">?</span>". </p><p>Slavic is asked to change each "<span class="tex-font-style-tt">?</span>" to a lowercase English letter such that string $t$ becomes a subsequence (not necessarily continuous) of the string $s$. </p><p>Output any such string, or say that it is impossible in case no string that respects the conditions exists.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \leq T \leq 10^4$)&nbsp;〞 the number of test cases.</p><p>The first line of each test case contains a single string $s$ ($1 \leq |s| \leq 2 \cdot 10^5$, and $s$ consists only of lowercase English letters and "<span class="tex-font-style-tt">?</span>"-s) &nbsp;每 the original string you have.</p><p>The second line of each test case contains a single string $t$ ($1 \leq |t| \leq |s|$, and $t$ consists only of lowercase English letters) &nbsp;每 the string that should be a subsequence of string $s$.</p><p>The sum of $|s|$ over all test cases doesn't exceed $2 \cdot 10^5$, where $|x|$ denotes the length of the string $x$.</p></div><div class="output-specification"><p>For each test case, if no such string exists as described in the statement, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output one line&nbsp;〞 the string that respects all conditions.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If multiple answers are possible, you can output any of them.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \leq T \leq 10^4$)&nbsp;〞 the number of test cases.</p><p>The first line of each test case contains a single string $s$ ($1 \leq |s| \leq 2 \cdot 10^5$, and $s$ consists only of lowercase English letters and "<span class="tex-font-style-tt">?</span>"-s) &nbsp;每 the original string you have.</p><p>The second line of each test case contains a single string $t$ ($1 \leq |t| \leq |s|$, and $t$ consists only of lowercase English letters) &nbsp;每 the string that should be a subsequence of string $s$.</p><p>The sum of $|s|$ over all test cases doesn't exceed $2 \cdot 10^5$, where $|x|$ denotes the length of the string $x$.</p>

## Output

<p>For each test case, if no such string exists as described in the statement, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" (without quotes). Then, output one line&nbsp;〞 the string that respects all conditions.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p><p>If multiple answers are possible, you can output any of them.</p>





```input1|2,3,6,7,10,11
5
?????
xbx
ab??e
abcde
ayy?x
a
ab??e
dac
paiu
mom
```




```output1
YES
xabax
YES
abcde
YES
ayyyx
NO
NO
```


