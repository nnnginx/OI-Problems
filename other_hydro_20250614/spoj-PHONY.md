<p>
You are chief debugger for Poorly Guarded Privacy, Inc. One of the top
selling product, ReallySecureAgent©, seems to have a problem with
its prime number generator. It produces from time to time bogus primes
N.
<br>
After a while, you realize that the problem is due to the way primes
are recognized.
<br>
<!-- MATH
$N = p_1 * p_2 * ... * p_k$
-->Every phony prime N you
discover can be characterized as follows. It is
odd and has distinct prime factors, say <img width="144" height="30" align="middle" border="0" src="/content/ak15:img1.png" alt="$ N = p_1 * p_2 * ... * p_k$"><!-- MATH
$p_ine p_j$
--> with <img width="53" height="30" align="middle" border="0" src="/content/ak15:img2.png" alt="$ p_ine p_j$">, where the number k of factors is at least 3.
Moreover, for all i=1..k, <img width="45" height="29" align="middle" border="0" src="/content/ak15:img3.png" alt="$ p_i-1$"> divides N-1. For instance,
561 = 3*11*17 is a phony prime.
<br>
<!-- MATH
$[N_{min},N_{max}[$
-->Intrigued by this phenomenon, you
decide to write a program that
enumerates all such N's in a given interval <img width="92" height="32" align="middle" border="0" src="/content/ak15:img4.png" alt="$ [N_{min},N_{max}[$"><!-- MATH
$1 le N_{min} < N_{max} < 2^31, N_{max}-N_{min} < 10^6$
-->
with <img width="313" height="34" align="middle" border="0" src="/content/ak15:img5.gif" alt="$ 1 le N_{min} &amp;amp;amp;amp;amp;lt; N_{max} &amp;amp;amp;amp;amp;lt; 2^31, N_{max}-N_{min} &amp;amp;amp;amp;amp;lt; 10^6$">.<br>
<b>Please note, that the source code limit for this problem is 2000 Bytes to avoid precalculated tables.</b>
</p>
<h3>Input</h3>
<p>
Each test case contains one line. On this line are written two
integers <img width="39" height="30" align="middle" border="0" src="/content/ak15:img6.png" alt="$ N_{min}$"> and <img width="41" height="30" align="middle" border="0" src="/content/ak15:img7.png" alt="$ N_{max}$"> separated
by a blank. The end of the input is signalled by a line containing two
zeros. The number of test cases is approximately 2000.
<br>
</p>
<h3>Output</h3>
<p>
For each test case, output the list of phony primes in increasing order, one per line. If there are no phony primes in the interval, then simply output none on a line.
</p>
<h3>Example</h3>
<div align="left">
<h4>Input:</h4>
<pre>10 2000
20000 21000
0 0
</pre>
<h4>Output:</h4>
<pre>561
1105
1729
none
</pre>
</div>