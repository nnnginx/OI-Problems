<p>For n positive integer, let <strong><em>F(n) = 1! ¡Á 2! ¡Á 3! ¡Á 4! ¡Á ... ¡Á n!</em></strong>, product of factorial(i) for i in [1..n].<br>

<br>
Let <strong><em>G(n) = {i in [1..n], such that n divides F(i)}</em></strong>. <br>

<br>
	It is obvious that <strong><em>n</em></strong> belongs to <strong><em>G(n)</em></strong> that makes it a non empty set.



</p><h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
an integer <strong><em>n</em></strong>.
</p>

<h3>Output</h3>
<p>For each test case, you have to print <strong><em>min(G(n))</em></strong>.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
4
5
6
</pre>
<pre><strong>Output:</strong>
3
5
3
</pre>

<h3>Explanation</h3>
<p>For test case #1:<br>
F(1) = 1! = 1 , not divisible by 4<br>
F(2) = 1! ¡Á 2! = 2 , not divisible by 4<br>
F(<b>3</b>) = 1! ¡Á 2! ¡Á 3! = 12 , <b>divisible</b> by 4<br>
F(4) = 1! ¡Á 2! ¡Á 3! ¡Á 4! = 288 , divisible by 4<br>
So G(4) = {<b>3</b>, 4}.</p>


<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^4
0 &lt; n &lt; 10^9
</pre>
<p>A little kB of Python code can get AC in half the time limit. (Edit 2017-02-11, after the compiler changes.)<br>
Input is not randomly chosen ;-) Have fun.</p>