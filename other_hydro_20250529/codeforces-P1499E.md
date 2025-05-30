## Description

<div><p>You are given two strings $x$ and $y$, both consist only of lowercase Latin letters. Let $|s|$ be the length of string $s$.</p><p>Let's call a sequence $a$ a merging sequence if it consists of exactly $|x|$ zeros and exactly $|y|$ ones in some order.</p><p>A merge $z$ is produced from a sequence $a$ by the following rules: </p><ul> <li> if $a_i=0$, then remove a letter from the beginning of $x$ and append it to the end of $z$; </li><li> if $a_i=1$, then remove a letter from the beginning of $y$ and append it to the end of $z$. </li></ul><p>Two merging sequences $a$ and $b$ are different if there is some position $i$ such that $a_i \neq b_i$.</p><p>Let's call a string $z$ <span class="tex-font-style-it">chaotic</span> if for all $i$ from $2$ to $|z|$ $z_{i-1} \neq z_i$.</p><p>Let $s[l,r]$ for some $1 \le l \le r \le |s|$ be a substring of consecutive letters of $s$, starting from position $l$ and ending at position $r$ inclusive.</p><p>Let $f(l_1, r_1, l_2, r_2)$ be the number of different merging sequences of $x[l_1,r_1]$ and $y[l_2,r_2]$ that produce <span class="tex-font-style-it">chaotic</span> merges. Note that only non-empty substrings of $x$ and $y$ are considered.</p><p>Calculate $\sum \limits_{1 \le l_1 \le r_1 \le |x| \\ 1 \le l_2 \le r_2 \le |y|} f(l_1, r_1, l_2, r_2)$. Output the answer modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a string $x$ ($1 \le |x| \le 1000$).</p><p>The second line contains a string $y$ ($1 \le |y| \le 1000$).</p><p>Both strings consist only of lowercase Latin letters.</p></div><div class="output-specification"><p>Print a single integer&nbsp;�� the sum of $f(l_1, r_1, l_2, r_2)$ over $1 \le l_1 \le r_1 \le |x|$ and $1 \le l_2 \le r_2 \le |y|$ modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a string $x$ ($1 \le |x| \le 1000$).</p><p>The second line contains a string $y$ ($1 \le |y| \le 1000$).</p><p>Both strings consist only of lowercase Latin letters.</p>

## Output

<p>Print a single integer&nbsp;�� the sum of $f(l_1, r_1, l_2, r_2)$ over $1 \le l_1 \le r_1 \le |x|$ and $1 \le l_2 \le r_2 \le |y|$ modulo $998\,244\,353$.</p>

## Samples

```input1
aaa
bb
```

```output1
24
```






```input2
code
forces
```

```output2
1574
```






```input3
aaaaa
aaa
```

```output3
0
```






```input4
justamassivetesttocheck
howwellyouhandlemodulooperations
```

```output4
667387032
```




## Note

<p>In the first example there are: </p><ul> <li> $6$ pairs of substrings "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">b</span>", each with valid merging sequences "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">10</span>"; </li><li> $3$ pairs of substrings "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">bb</span>", each with a valid merging sequence "<span class="tex-font-style-tt">101</span>"; </li><li> $4$ pairs of substrings "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">b</span>", each with a valid merging sequence "<span class="tex-font-style-tt">010</span>"; </li><li> $2$ pairs of substrings "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">bb</span>", each with valid merging sequences "<span class="tex-font-style-tt">0101</span>" and "<span class="tex-font-style-tt">1010</span>"; </li><li> $2$ pairs of substrings "<span class="tex-font-style-tt">aaa</span>" and "<span class="tex-font-style-tt">b</span>", each with no valid merging sequences; </li><li> $1$ pair of substrings "<span class="tex-font-style-tt">aaa</span>" and "<span class="tex-font-style-tt">bb</span>" with a valid merging sequence "<span class="tex-font-style-tt">01010</span>"; </li></ul><p>Thus, the answer is $6 \cdot 2 + 3 \cdot 1 + 4 \cdot 1 + 2 \cdot 2 + 2 \cdot 0 + 1 \cdot 1 = 24$.</p>
