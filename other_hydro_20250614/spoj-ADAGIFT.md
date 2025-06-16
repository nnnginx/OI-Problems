<p>Even though there is almost half a year before Ada the Ladybug's birthday, her friend already started searching for a birthday gift. As Ada is a mathematician, they decided to give her a number. They know that Ada loves numbers, which are composed by concatenation of prime numbers (at least one).</p>
<p>Sometime there are multiple ways to do so: for example 37 can be concatenation of "3" and "7", yet it can also be concatenation of "37" itself. The more ways, the better the number is. Ada's friends want to surprise her by as good number as possible so they want you to write a program, which could count the number of ways.</p>
<p><b>NOTE:</b>Number with leading zeroes is a valid number (treat it as if the leading zeroes are not there)

</p><h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü T ¡Ü 100</strong></p>
<p>Each of the next <strong>N</strong> lines contains a number <strong>1 ¡Ü A &lt;     10<sup>30</sup></strong></p>
<h3>Output</h3>
<p>For each number, print the number of ways it can be written as concatenation of prime numbers.</p>
<h3>Example Input</h3>
<pre>8
2
37
111
3737
133
1000000009
113731191937237
1111111111111111111111
</pre>
<h3>Example Output</h3>
<pre>1
2
0
6
1
1
197
1
</pre>