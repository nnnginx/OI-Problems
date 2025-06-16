## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p>Timofey is writing a competition called Capture the Flag (or CTF for short). He has one task left, which involves hacking a security system. The entire system is based on polynomial hashes$^{\text{∗}}$.</p><p>Timofey can input a string consisting of lowercase Latin letters into the system, and the system will return its polynomial hash. To hack the system, Timofey needs to find the polynomial hash parameters ($p$ and $m$) that the system uses.</p><p>Timofey doesn't have much time left, so he will only be able to make $3$ queries. Help him solve the task.</p><div class="statement-footnote"><p>$^{\text{∗}}$ The polynomial hash of a string $s$, consisting of lowercase Latin letters of length $n$, based on $p$ and modulo $m$ is $(\mathrm{ord}(s_1) \cdot p ^ 0 + \mathrm{ord}(s_2) \cdot p ^ 1 + \mathrm{ord}(s_3) \cdot p ^ 2 + \ldots + \mathrm{ord}(s_n) \cdot p ^ {n - 1}) \bmod m$. Where $s_i$ denotes the $i$-th character of the string $s$, $\mathrm{ord}(\mathrm{chr})$ denotes the ordinal number of the character $\mathrm{chr}$ in the English alphabet, and $x \bmod m$ is the remainder of $x$ when divided by $m$.</p></div></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p><span class="tex-font-style-bf">It is guaranteed that the $p$ and $m$ used by the system satisfy the conditions: $26 &lt; p \leq 50$ and $p + 1 &lt; m \leq 2 \cdot 10^9$.</span></p></div><div><h2>Interaction</h2><p>To make a query to the system, output <span class="tex-font-style-tt">?</span> $s$, where $s$ is a string of <span class="tex-font-style-bf">no more than</span> $50$ characters in length, the hash of which you want to know. In response to this query, you will receive the polynomial hash of the string $s$.</p><p>To output the answer, output <span class="tex-font-style-tt">!</span> $p$ $m$, where $p$ is the base of the hash, and $m$ is the modulus. After that, immediately proceed to the next test case.</p><p>You have to make not more than $3$ queries <span class="tex-font-style-tt">?</span>, otherwise you will get verdict <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>After outputting a query, do not forget to output a newline and flush the output buffer. Otherwise, you will receive the verdict <span class="tex-font-style-tt">Idleness limit exceeded</span>. To flush the buffer, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see the documentation for other languages. </li></ul></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^3$)&nbsp;— the number of test cases.</p><p><span class="tex-font-style-bf">It is guaranteed that the $p$ and $m$ used by the system satisfy the conditions: $26 &lt; p \leq 50$ and $p + 1 &lt; m \leq 2 \cdot 10^9$.</span></p>





```input1
1

32

28
```




```output1
? aa

? yb

! 31 59
```



## Note

<p>Answer for the first query is $(ord(a) \cdot 31^0 + ord(a) \cdot 31^1) \mod 59 = (1 + 1 \cdot 31) \mod 59 = 32$.</p><p>Answer for the second query is $(ord(y) \cdot 31^0 + ord(b) \cdot 31^1) \mod 59 = (25 + 2 \cdot 31) \mod 59 = 28$.</p>
