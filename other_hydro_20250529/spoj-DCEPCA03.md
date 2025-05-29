<p>Given the value of N, you will have to find the value of H. The meaning of H is given in the following code:</p>

<p><tt>
H=0;<br>
For (i=1; i&lt;=n; i++) {<br>
&nbsp;&nbsp;&nbsp;&nbsp;For (j=1; j&lt;=n; j++) {<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;H = H + totient(i) * totient(j);<br>
&nbsp;&nbsp;&nbsp;&nbsp;}<br>
}
</tt></p>

<p><strong>Totient</strong> or phi function, ¦Õ(n) is an arithmetic function that counts the number of positive integers less than or equal to n that are relatively prime to n. That is, if n is a positive integer, then ¦Õ(n) is the number of integers k in the range 1 ¡Ü k ¡Ü n for which gcd(n, k) = 1</p>

<h3>Constraints</h3>
<p>0 &lt; T &lt;= 50<br>0 &lt; N &lt;= 10^4</p>

<h3>Input</h3>
<p>The first line contains T, the number of test cases. It is followed by T lines each containing a number N .</p>

<h3>Output</h3>
<p>For each line of input produce one line of output. This line contains the value of H for the corresponding N.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
10

<strong>Output:</strong>
16
1024</pre>