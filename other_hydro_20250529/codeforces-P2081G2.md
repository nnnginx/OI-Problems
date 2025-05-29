## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that in this version, the limit on $n$ and the <span class="tex-font-style-it">time limit</span> are higher. You can hack only if you solved all versions of this problem.</span> </p><p>You are given an integer $n$, and you need to compute $(\sum_{k=1}^n k\bmod\varphi(k))\bmod 2^{32}$, where $\varphi(k)$ equals the number of positive integers no greater than $k$ that are coprime with $k$.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \le n \le 10^{12}$).</p></div><div class="output-specification"><p>Print a single integer, representing $(\sum_{k=1}^n k\bmod\varphi(k))\bmod 2^{32}$.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \le n \le 10^{12}$).</p>

## Output

<p>Print a single integer, representing $(\sum_{k=1}^n k\bmod\varphi(k))\bmod 2^{32}$.</p>





```input1|
5
```




```input2|
10000000
```




```input3|
10000000000
```




```output1
2
```




```output2
2316623097
```




```output3
282084447
```


