## Description

<div><p><span class="tex-font-style-it">I, Fischl, Prinzessin der Verurteilung, descend upon this land by the call of fate an �� Oh, you are also a traveler from another world?</span> <span class="tex-font-style-it">Very well, I grant you permission to travel with me.</span></p><p>It is no surprise Fischl speaks with a strange choice of words. However, this time, not even Oz, her raven friend, can interpret her expressions! Maybe you can help us understand what this young princess is saying?</p><p>You are given a string of $n$ lowercase Latin letters, the word that Fischl just spoke. You think that the MEX of this string may help you find the meaning behind this message. The MEX of the string is defined as the shortest string that <span class="tex-font-style-bf">doesn't</span> appear as a contiguous substring in the input. If multiple strings exist, the lexicographically smallest one is considered the MEX. Note that the empty substring does NOT count as a valid MEX.</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul><p>A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters from the beginning and several (possibly, zero or all) characters from the end.</p><p>Find out what the MEX of the string is!</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 1000$)&nbsp;�� the length of the word. The second line for each test case contains a single string of $n$ lowercase Latin letters.</p><p>The sum of $n$ over all test cases will not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output the MEX of the string on a new line.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 1000$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 1000$)&nbsp;�� the length of the word. The second line for each test case contains a single string of $n$ lowercase Latin letters.</p><p>The sum of $n$ over all test cases will not exceed $1000$.</p>

## Output

<p>For each test case, output the MEX of the string on a new line.</p>

## Samples

```input1
3
28
qaabzwsxedcrfvtgbyhnujmiklop
13
cleanairactbd
10
aannttoonn
```

```output1
ac
f
b
```



