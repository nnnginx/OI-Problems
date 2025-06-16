<p><span style="font-size: small;">You are living in a city build entirely of power towers such as 3^3^3 and 10^10^10^10. To enter a building you must type the last 9 digits of the number represented by the tower, written in decimal form, on a keypad next to the main entrance. You are not sharp enough at mental maths, but you can write a handy program to bring along in your pocket.</span></p>
<p><span style="font-size: small;">A power tower is defined as repeated exponentiation. We write this using <a href="http://en.wikipedia.org/wiki/Knuth's_up-arrow_notation">Knuth's up-arrow notation</a> as: e¡ü¡üa = e^e^...^e (a terms). Remember that ^ (exponentiation) is right assosiative. For example: 2¡ü¡ü4 = 2^2^2^2 =&nbsp;2^(2^(2^2)) = 2^2^4 = 2^16 = 65536, and 3¡ü¡ü1 = 3. The value of a tower of heigh 0 is 1.</span></p>
<h3>Input</h3>
<p><span style="font-size: small;">The first line contains integer C in [0..1000], the number of test cases.</span></p>
<p><span style="font-size: small;">Then follows C lines, each with integers e,a in [0..2147483647]. (non-negative 32-bit ints).</span></p>
<h3>Output</h3>
<p><span style="font-size: small;">For each testcase output e¡ü¡üa, or if the output has more than 9 digits, output "..." and then the last 9 digits.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre>3</pre>
<pre>0 0</pre>
<pre>2 5</pre>
<pre>993306745 75707320

<strong><strong>Output:</strong></strong>
</pre>
<pre>1</pre>
<pre>...719156736</pre>
<pre>...884765625</pre>