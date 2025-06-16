## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. In this version $l\le r$.</span></p><p>You are given a string $s$. For a fixed $k$, consider a division of $s$ into exactly $k$ continuous substrings $w_1,\dots,w_k$. Let $f_k$ be the maximal possible $LCP(w_1,\dots,w_k)$ among all divisions.</p><p>$LCP(w_1,\dots,w_m)$ is the length of the Longest Common Prefix of the strings $w_1,\dots,w_m$.</p><p>For example, if $s=abababcab$ and $k=4$, a possible division is $\color{red}{ab}\color{blue}{ab}\color{orange}{abc}\color{green}{ab}$. The $LCP(\color{red}{ab},\color{blue}{ab},\color{orange}{abc},\color{green}{ab})$ is $2$, since $ab$ is the Longest Common Prefix of those four strings. Note that each substring consists of a continuous segment of characters and each character belongs to <span class="tex-font-style-bf">exactly</span> one substring.</p><p>Your task is to find $f_l,f_{l+1},\dots,f_r$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$, $r$ ($1 \le l \le r \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string and the given range.</p><p>The second line of each test case contains string $s$ of length $n$, all characters are lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output $r-l+1$ values: $f_l,\dots,f_r$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains two integers $n$, $l$, $r$ ($1 \le l \le r \le n \le 2 \cdot 10^5$)&nbsp;！ the length of the string and the given range.</p><p>The second line of each test case contains string $s$ of length $n$, all characters are lowercase English letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output $r-l+1$ values: $f_l,\dots,f_r$.</p>





```input1|2,3,6,7,10,11,14,15
7
3 1 3
aba
3 2 3
aaa
7 1 5
abacaba
9 1 6
abababcab
10 1 10
aaaaaaawac
9 1 9
abafababa
7 2 7
vvzvvvv
```




```output1
3 1 0 
1 1 
7 3 1 1 0 
9 2 2 2 0 0 
10 3 2 1 1 1 1 1 0 0 
9 3 2 1 1 0 0 0 0 
2 2 1 1 1 0
```


