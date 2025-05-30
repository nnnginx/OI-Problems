## Description

<div><p>A palindrome is a string that reads the same backward as forward. For example, the strings "<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aba</span>", and "<span class="tex-font-style-tt">abccba</span>" are palindromes, but "<span class="tex-font-style-tt">codeforces</span>" and "<span class="tex-font-style-tt">ab</span>" are not. You hate palindromes because they give you d��j�� vu.</p><p>There is a string $s$. You <span class="tex-font-style-bf">must</span> insert <span class="tex-font-style-bf">exactly one</span> character '<span class="tex-font-style-tt">a</span>' somewhere in $s$. If it is possible to create a string that is <span class="tex-font-style-bf">not</span> a palindrome, you should find one example. Otherwise, you should report that it is impossible.</p><p>For example, suppose $s=$ "<span class="tex-font-style-tt">cbabc</span>". By inserting an '<span class="tex-font-style-tt">a</span>', you can create "<span class="tex-font-style-tt">acbabc</span>", "<span class="tex-font-style-tt">cababc</span>", "<span class="tex-font-style-tt">cbaabc</span>", "<span class="tex-font-style-tt">cbabac</span>", or "<span class="tex-font-style-tt">cbabca</span>". However "<span class="tex-font-style-tt">cbaabc</span>" is a palindrome, so you must output one of the other options.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The only line of each test case contains a string $s$ consisting of lowercase English letters.</p><p>The total length of all strings does not exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no solution, output "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" followed by your constructed string of length $|s|+1$ on the next line. If there are multiple solutions, you may print any.</p><p>You can print each letter of "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$) �� the number of test cases.</p><p>The only line of each test case contains a string $s$ consisting of lowercase English letters.</p><p>The total length of all strings does not exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case, if there is no solution, output "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, output "<span class="tex-font-style-tt">YES</span>" followed by your constructed string of length $|s|+1$ on the next line. If there are multiple solutions, you may print any.</p><p>You can print each letter of "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (upper or lower).</p>

## Samples

```input1
6
cbabc
ab
zza
ba
a
nutforajaroftuna
```

```output1
YES
cbabac
YES
aab
YES
zaza
YES
baa
NO
YES
nutforajarofatuna
```




## Note

<p>The first test case is described in the statement.</p><p>In the second test case, we can make either "<span class="tex-font-style-tt">aab</span>" or "<span class="tex-font-style-tt">aba</span>". But "<span class="tex-font-style-tt">aba</span>" is a palindrome, so "<span class="tex-font-style-tt">aab</span>" is the only correct answer.</p><p>In the third test case, "<span class="tex-font-style-tt">zaza</span>" and "<span class="tex-font-style-tt">zzaa</span>" are correct answers, but not "<span class="tex-font-style-tt">azza</span>".</p><p>In the fourth test case, "<span class="tex-font-style-tt">baa</span>" is the only correct answer.</p><p>In the fifth test case, we can only make "<span class="tex-font-style-tt">aa</span>", which is a palindrome. So the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the sixth test case, "<span class="tex-font-style-tt">anutforajaroftuna</span>" is a palindrome, but inserting '<span class="tex-font-style-tt">a</span>' elsewhere is valid.</p>
