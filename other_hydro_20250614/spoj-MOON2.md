<p>
<a href="http://en.wikipedia.org/wiki/Air_(French_band)">Air</a> is a music duo from France.<br>
You will be told the secret of the critically acclaimed album 
<a href="http://en.wikipedia.org/wiki/Moon_Safari">Moon Safari</a>: mathematics.<br>
The goal of your new task is to compute an ethereal sum.</p>
<img title="AirSum" src="../../content/francky:AirSum" alt="AirSum">
<p>Three trips on the moon are provided,
<a href="http://www.spoj.com/problems/MOON/">Moon</a> (easy),
<a href="http://www.spoj.com/problems/MOON1/">Moon1</a> (medium),
<a href="http://www.spoj.com/problems/MOON2/">Moon2</a> (hard)
with different constraints.</p>


<h3>Input</h3>
<p>The first line contains an integer <em>T</em>, the number of test cases.<br>
On the next <em>T</em> lines, you will be given three integers <em>N</em>, <em>a</em> and <em>r</em>.<br>
</p>

<h3>Output</h3>
<p>Output <em>T</em> lines, one for each test case, with <em>S<sub>N,a,r</sub></em> = sum( <em>a^i i^r</em>, for <em>i</em> in [<em>1..N</em>] ).<br>
Since the answer can get very big, output it modulo 10<sup>9</sup>+7.</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
3 4 5
6 7 8

<b>Output:</b>
16068
329990641
</pre>

<h3>Explanation</h3>
<p>
The first case is, with <em>N</em>=3, <em>a</em>=4, <em>r</em>=5, about the sum :
4^1 ¡Á 1^5 +
4^2 ¡Á 2^5 +
4^3 ¡Á 3^5 = 4 + 512 + 15552 = <b>16068</b>.<br>

The second case is, with <em>N</em>=6, <em>a</em>=7, <em>r</em>=8, about the sum :
7^1 ¡Á 1^8 +
7^2 ¡Á 2^8 +
7^3 ¡Á 3^8 +
7^4 ¡Á 4^8 +
7^5 ¡Á 5^8 +
7^6 ¡Á 6^8 +
7^7 ¡Á 7^8 = 204329992069 ¡Ô <b>329990641</b> (mod 10^9+7).<br>

</p>

<h3>Constraints</h3>
<pre>0 &lt; T¡Ár &lt; 2 560 000
1 &lt; N &lt; 10^9
1 &lt; a &lt; 10^9
</pre>
<p>
Uniform random input in the range.<br>
More precise information : there are 5 input files.<br>
In0 : T&lt;20000 and r &lt;= 128<br>
In1 : T&lt;2000 and r &lt;= 1250<br>
In2 : T&lt;200 and r &lt;= 11000<br>
In3 : T&lt;20 and r &lt;= 100000<br>
In4 : T&lt;2 and r &lt;= 1000000<br>
</p>

<h3>Information</h3>
<p>This trip can be done with a O(T¡Ár¡Álog(N)) method and some interpreted languages.<br>
Edited(2017-02-11, after compiler changes).<br>
My non optimal Py3 code got AC under 5s for each of the 5 input files.<br>
@speed addicts : My fastest C code got AC in 0.42s. (approx 0.08s per file)<br>
Good luck and have fun ;-)
</p>