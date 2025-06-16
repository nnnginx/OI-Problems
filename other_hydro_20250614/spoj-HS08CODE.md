<p>Today, Gerrob's RSA company has featured a New RSA cryptosystem: its public key is <em>n</em>, the secret keys are three distinct primes <em>p</em>, <em>q</em> and <em>r</em>, where <em>n</em>=<em>p</em>*<em>q</em>*<em>r</em>. Note that the ordinary RSA uses only 2 primes! Unfortunately some hackers have stolen a DVD from the company. It does not store the secret keys, only some information about the system, namely, the values of: <br> ¦Õ (<em>n</em>) - Euler's totient function and  <br> ¦Ò (<em>n</em>) - the sum of the divisors.<br> Obviously you know also <em>n</em>, because that's public.</p>
<p>Now, Gerrob's RSA employees are trying to determine  if hackers will be able to break the system. Could you help them to answer this question?</p>
<h3>Input</h3>
<p>The first line contains a single integer <em>T</em>, the number of test cases, where <em>T</em>¡Ü 20000. The following <em>T</em> lines each contains three numbers n, ¦Õ (<em>n</em>) and ¦Ò (<em>n</em>) in this order. There are 5 input sets.</p>
<h3>Output</h3>
<p>Output <em>T</em> lines, the values of <em>p</em>, <em>q</em> and <em>r</em> in increasing order. It is guaranteed that <em>p</em>, <em>q</em>, <em>r</em>&lt;10<sup>6</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
30 8 72
61321 54912 68040
451464315257 451286179344 451642497600
91896729624994213 91896040105364880 91897419147616160
<strong>Output:</strong>
2 3 5
13 53 89
6397 8039 8779
231859 574261 690187
</pre>
<p><strong>Warning: large input/output data, be careful with certain languages </strong> <br><br></p>
<p><strong>Warning: A naive algorithm will probably solve only the first input set. </strong></p>