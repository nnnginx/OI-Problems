<p>Perfect squares are fairly simple concept. A number like 49 is perfect sqaure because it can be written as product of two same natural number i.e. 7 * 7.</p>
<p>On the other hand infinite sequence of numbers can be considered an intriguing concept, because it is not possible to represent all numbers belonging in an infinite sequence easily.</p>
<p>Can read more about infinite sequences <a href="https://en.wikipedia.org/wiki/Sequence#Finite_and_infinite">here</a>.</p>
<p>So one way to represent infinte sequnece of numbers is to use an algebraic expression instead of writing all numbers in the sequence.</p>
<p>For example, expression x<sup>2</sup>&nbsp;+ 1 represents the series 2, 5, 10, 17, .... . (Substituting value of x = 1, 2, 3, ... to get the values in the sequence)</p>
<p>Similarly x<sup>2</sup>&nbsp;+ 4 represents the infinite series 5, 8, 13, 20, .... (Substituting value of x = 1, 2, 3, ... to get the values in the sequence)</p>
<p>Given an infinte sequence of numbers of form x<sup>2</sup>&nbsp;+ n, figuring out perfect square numbers within this sequence can be challenging even if checking a number is perfect square is easy.</p>
<p>For example, consider the infinite sequence represented by x<sup>2</sup>&nbsp;+ 771401, only when x = 385700 then x<sup>2</sup>&nbsp;+ 771401 = 148765261401 = 385701<sup>2</sup>&nbsp;is a perfect square. There are no other values of x for which x<sup>2</sup>&nbsp;+ 771401 will be a square.</p>
<p>This is because 771401 is difference between two consecutive squares 385700<sup>2</sup>&nbsp;and 385701<sup>2</sup>&nbsp;. So the infinite sequence represented by x<sup>2</sup>&nbsp;+ 771401 has only 1 perfect sqaure number when x = 385701.</p>
<p>Let us consider one more example x<sup>2</sup>&nbsp;+ 45, only when x = 2, 6 or 22 then x<sup>2</sup>&nbsp;+ 45 is a perfect square. So the infinite sequence represented by x<sup>2</sup>&nbsp;+ 45 has only 3 perfect sqaure numbers when x = 2, 6 or 22.</p>
<p>But infinite sequence represented by x<sup>2</sup>&nbsp;+ 46 contains no prefect square numbers, this because if it contains such a number then infinite sequence represented x<sup>2</sup>&nbsp;+ 45 will not have any perfect sqaure numbers which is a contradiction</p>
<p>because we know 3 perfect square numbers contained in infinite sequence represented by x<sup>2</sup>&nbsp;+ 45 .</p>
<p>In other words given equation x<sup>2</sup>&nbsp;+ n where n is a whole number (i.e. n can take values like 0,1,2,3,4....) find all x in ascending order such that x<sup>2</sup>&nbsp;+ n is a perfect square</p>
<h3>Input</h3>
<p>The first line of input file contains a positive integer 't' and next 't' lines contains a string which looks like 'x^2 + n' (example 'x^2 + 3', 'x^2 + 5' etc.).</p>
<p>0 &lt;= n &lt;= 10<sup>6</sup>&nbsp;</p>
<p>Sum of all 'n' in a test file will not exceed 10<sup>6</sup></p>
<h3>Output</h3>
<p>The output line has to printed for each test case line.</p>
<p>If there are finite number of values of 'x' for which x<sup>2</sup>&nbsp;+ n is a perfect square then print all such x in ascending order seperated by comma and space (, ) and enclosed within sqaure brackets. So for 'x^2 + 45' the output line will look like [2, 6, 22].</p>
<p>Incase there are no such values of 'x' for which x<sup>2</sup>&nbsp;+ n is a perfect square then print "No Solution" (without quotes and case sensitive). So for 'x^2 + 46' the output line will be "No Solution".</p>
<p>Incase there are infinitely many solutions for which x<sup>2</sup>&nbsp;+ n is a perfect square then print "Infinitely Many Solutions" (without quotes and case sensitive). So for 'x^2 + 0' the output line will be "Infinitely Many Solutions"</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
</pre>
<pre>3</pre>
<pre>x^2 + 45</pre>
<pre>x^2 + 0</pre>
<pre>x^2 + 46</pre>
<pre><strong>Output:</strong>
</pre>
<pre>[2, 6, 22]</pre>
<pre>Infinitely Many Solutions</pre>
<pre>No Solution</pre>