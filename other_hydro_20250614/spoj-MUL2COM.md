<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MUL2COM/en/">English</a></td> 
<td width="50%"><a href="/problems/MUL2COM/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>In this problem, you have to multiply two n-bit binary numbers in 2s complement form. The result should be also a n-bit binary number in 2s complement form. In case there is an arithmetic overflow, you program should be able to detect it.</p>
<p>For your information, the 2s complement form of -x is the number 2^n-x. A n-bit 2s complement number ranges from -2<sup>n-1</sup> to 2<sup>n-1</sup>-1.</p>
<h3>Input</h3>
<p>There are multiple test cases (no more than 40). For each test case, there are three input lines. The first line contains n (0 ¡Ü n ¡Ü 1024). n=0 signals the end of the input. Otherwise, the second and third lines contain the two n-bit binary numbers.</p>
<h3>Output</h3>
<p>For each test case, output "overflow" if there is an arithmetic overflow. Otherwise, print the result in 2s complement form.</p>

<h3>Example</h3>
<pre><b>Input</b>
3
110
011
4
0011
1110
0

<b>Output</b>
overflow
1010
</pre>