<p>Given any string of decimal digits, ending in 1, 3, 7 or 9,&nbsp; there is always a decimal <br>number, which when cubed has a decimal expansion ending in the original given digit <br>string. The number need never have more digits than the given digit string.&nbsp; <br>&nbsp;<br>Write a program, which takes as input a string of decimal digits ending in 1, 3, 7 or 9 <br>and finds a number of at most the same number of digits, which when cubed, ends in <br>the given digit string.</p>
<h3>Input</h3>
<p>The input begins with a line containing only the count of problem instances, nProb, as a <br>decimal integer, 1 &lt;= nProb &lt;= 100.&nbsp; This is followed by nProb lines, each of which <br>contains a string of between 1 and 10 decimal digits ending in 1, 3, 7 or 9.</p>
<h3>Output</h3>
<p>For each problem instance, there should be one line of output consisting of the number, <br>which when cubed, ends in the given digit string. The number should be output as a <br>decimal integer with no leading spaces and no leading zeroes.&nbsp;</p>
<p>If there are many answers, the minimum should be chosen.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 <br>123 <br>1234567 <br>435621 <br>9876543213
<strong>Output:</strong>
947 <br>2835223 <br>786941 <br>2916344917</pre>