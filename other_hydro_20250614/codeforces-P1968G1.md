## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. In this version $l=r$.</span></p><p>You are given a string $s$. For a fixed $k$, consider a division of $s$ into exactly $k$ continuous substrings $w_1,\dots,w_k$. Let $f_k$ be the maximal possible $LCP(w_1,\dots,w_k)$ among all divisions.</p><p>$LCP(w_1,\dots,w_m)$ is the length of the Longest Common Prefix of the strings $w_1,\dots,w_m$.</p><p>For example, if $s=abababcab$ and $k=4$, a possible division is $\color{red}{ab}\color{blue}{ab}\color{orange}{abc}\color{green}{ab}$. The $LCP(\color{red}{ab},\color{blue}{ab},\color{orange}{abc},\color{green}{ab})$ is $2$, since $ab$ is the Longest Common Prefix of those four strings. Note that each substring consists of a continuous segment of characters and each character belongs to <span class="tex-font-style-bf">exactly</span> one substring.</p><p>Your task is to find $f_l,f_{l+1},\dots,f_r$. <span class="tex-font-style-bf">In this version $l=r$</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$, $r$ ($1 \le l = r \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string and the given range.</p><p>The second line of each test case contains string $s$ of length $n$, all characters are lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $r-l+1$ values: $f_l,\dots,f_r$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$, $r$ ($1 \le l = r \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string and the given range.</p><p>The second line of each test case contains string $s$ of length $n$, all characters are lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $r-l+1$ values: $f_l,\dots,f_r$.</p>





```input1|2,3,6,7,10,11,14,15
7
3 3 3
aba
3 3 3
aaa
7 2 2
abacaba
9 4 4
abababcab
10 1 1
codeforces
9 3 3
abafababa
5 3 3
zpozp
```




```output1
0
1
3
2
10
2
0
```



## Note

<p>In the first sample $n=k$, so the only division of $aba$ is $\color{red}a\color{blue}b\color{orange}a$. The answer is zero, because those strings do not have a common prefix.</p><p>In the second sample, the only division is $\color{red}a\color{blue}a\color{orange}a$. Their longest common prefix is one.</p>
