<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MDIGITS/en/">English</a></td> 
<td width="50%"><a href="/problems/MDIGITS/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>Given two integers a and b, we write the numbers between a and b, inclusive, in a list. Your task is to calculate the number of occurrences of each digit.</p>

<p>For example, if a = 1024 and b = 1032, the list will be 1024 1025 1026 1027 1028 1029 1030 1031 1032 there are ten 0s in the list, ten 1s, seven 2s, three 3s, and etc. </p>

<h3>Input</h3>
<p>The input consists of up to 500 lines. Each line contains two numbers a and b where 0 &lt; a, b &lt; 100000000. The input is terminated by a line 0 0.</p>

<h4>Sample Input</h4>
<pre>1 10
44 497
346 542
1199 1748
1496 1403
1004 503
1714 190
1317 854
1976 494
1001 1960
0 0</pre>

<h3>Output</h3>
<p>For each pair of input, output a line containing ten numbers separated by single spaces. The first number is the number of occurrences of the digit 0, the second is the number of occurrences of the digit 1, etc</p>

<h4>Sample output</h4>
<pre>1 2 1 1 1 1 1 1 1 1
85 185 185 185 190 96 96 96 95 93
40 40 40 93 136 82 40 40 40 40
115 666 215 215 214 205 205 154 105 106
16 113 19 20 114 20 20 19 19 16
107 105 100 101 101 197 200 200 200 200
413 1133 503 503 503 502 502 417 402 412
196 512 186 104 87 93 97 97 142 196
398 1375 398 398 405 499 499 495 488 471
294 1256 296 296 296 296 287 286 286 247</pre>

<p><b>Note : wrong dataset index, rejugded and TLE some ACed code</b></p>