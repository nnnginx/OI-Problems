<h3>Factorial(N) in base B : The number of trailing zeros.</h3>

<p>
Factorial(<b>19</b>) in base <b>9</b>¡Á10^<b>0</b>=9 can be written 72573550063508<b>0000</b>, ending with <b>4</b> zeros.
<br>
Factorial(<b>43</b>) in base <b>2</b>¡Á10^<b>1</b>=20 can be written 59HHHFECFCCEGH5G7I7A3A8G88F8CD8G<b>000000000</b>, ending with <b>9</b> zeros.
<br>
What about working with serious constraints and tricky cases ?<br>
Factorial(<b>N</b>) will be a huge one, the base will be dummy too and have the special form : <b>B</b>¡Á10^<b>E</b>.
</p>


<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are three integers : N, B, E.</p>

<h3>Output</h3>
<p>
For each test case, print the number of zeros at the end of Factorial(N) written in base B¡Á10^E.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
19 9 0
43 2 1
10000 100 10

<b>Output:</b>
4
9
208
</pre>

<h3>Constraints</h3>
<pre>1 &lt;= T &lt; 2000
1 &lt;= N &lt; 10^1000
1 &lt;= B &lt; 10^9
0 &lt;= E &lt; 10^9
</pre>

<h3>Informations</h3>
<p>Don't worry about the 'special' base 1 (B=1 and E=0), it is absent from input.
<br>
About distribution : random input (N : log-uniform, B : uniform, E : uniform) in their range. Some tricky cases are added.
<br>
It is recommended to solve <a href="http://www.spoj.com/problems/FACTBASE/">FACTBASE</a> first, and find a way to solve
<a href="http://www.spoj.com/problems/FCTRL/">FCTRL</a> much faster than common solutions.
<br> Time limit is ¡Á13.6 my best Python3 time, or ¡Á1.33 my "basic" one.
</p>