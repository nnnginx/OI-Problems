<p>One of the famous proofs of modern mathematics is Georg Cantor's demonstration that the set of rational numbers is enumerable. The proof works by using an explicit enumeration of rational numbers as shown in the diagram below.</p>
<pre>1/1 1/2 1/3 1/4 1/5 ...
2/1 2/2 2/3 2/4
3/1 3/2 3/3
4/1 4/2
5/1
</pre>

<p>In the above diagram, the first term is 1/1, the second term is 1/2, the third term is 2/1, the fourth term is 3/1, the fifth term is 2/2, and so on.</p>

<h3>Input</h3>
<p>The input starts with a line containing a single integer <b>t</b> &lt;= 20, the number of test cases. <b>t</b> test cases follow. </p> <p>Then, it contains a single number per line.</p>

<h3>Output</h3>
<p>You are to write a program that will read a list of numbers in the range from 1 to 10^7 and will print for each number the corresponding term in Cantor's enumeration as given below.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
3
14
7

<b>Output:</b>
TERM 3 IS 2/1
TERM 14 IS 2/4
TERM 7 IS 1/4
</pre>