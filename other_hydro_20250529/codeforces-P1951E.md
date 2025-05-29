## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/d4iOF4yoNQw"><span class="tex-font-style-it">Christopher Tin ft. Soweto Gospel Choir - Baba Yetu</span></a></div><div class="epigraph-source">ඞ</div></div><p>You are given a string $s$ consisting of lowercase Latin characters. You need to partition$^\dagger$ this string into some substrings, such that each substring is not a palindrome$^\ddagger$.</p><p>$^\dagger$ A partition of a string $s$ is an ordered sequence of some $k$ strings $t_1, t_2, \ldots, t_k$, such that $t_1 + t_2 + \ldots + t_k = s$, where $+$ here represents the concatenation operation.</p><p>$^\ddagger$ A string $s$ is considered a palindrome if it reads the same backwards as forwards. For example, $\mathtt{racecar}$, $\mathtt{abccba}$, and $\mathtt{a}$ are palindromes, but $\mathtt{ab}$, $\mathtt{dokibird}$, and $\mathtt{kurosanji}$ are not.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains a string $s$ consisting of lowercase Latin characters ($1 \le |s| \le 10^6$).</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if there exists a partition of $s$ whose parts are not palindromes, or <span class="tex-font-style-tt">"NO"</span> if there is no such partition.</p><p>If the answer is <span class="tex-font-style-tt">"YES"</span>, on the second line, print an integer $k$&nbsp;— the number of parts that $s$ needs to be partitioned to such that each part is not a palindrome. On the third line, print $k$ strings $t_1, t_2, \ldots, t_k$ representing such a partition. If there are multiple such partitions, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains a string $s$ consisting of lowercase Latin characters ($1 \le |s| \le 10^6$).</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print on one line <span class="tex-font-style-tt">"YES"</span> if there exists a partition of $s$ whose parts are not palindromes, or <span class="tex-font-style-tt">"NO"</span> if there is no such partition.</p><p>If the answer is <span class="tex-font-style-tt">"YES"</span>, on the second line, print an integer $k$&nbsp;— the number of parts that $s$ needs to be partitioned to such that each part is not a palindrome. On the third line, print $k$ strings $t_1, t_2, \ldots, t_k$ representing such a partition. If there are multiple such partitions, print any of them.</p>





```input1|2,4
3
sinktheyacht
lllllllll
uwuowouwu
```




```output1
YES
1
sinktheyacht
NO
YES
3
uw uow ouwu
```



## Note

<p>In the first test case, since $\mathtt{sinktheyacht}$ is already non-palindrome, the partition $[\mathtt{sinktheyacht}]$ is valid.</p><p>In the second test case, as any substring of the string $s$ is palindrome, there are no valid partitions.</p><p>In the third test case, another valid partition is $[\mathtt{uw},\mathtt{uo}, \mathtt{wou}, \mathtt{wu}]$.</p>
