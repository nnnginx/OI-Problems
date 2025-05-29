<p>
You might have heard of the Fibonacci numbers and of the number <b>pi</b>. If you let these two ideas
merge, a new and esoteric concept comes into being: <b>the Pibonacci numbers</b>. These can be defined for
real <b>x&gt;=0</b> by:
</p>

<table width="90%" class="podklad2">
<tbody><tr>
<td nowrap=""><b>P(x) = 1</b></td>
<td>for <b>0&lt;=x&lt;4</b></td>
</tr>
<tr>
<td nowrap=""><b>P(x) = P(x-1) + P(x-pi)</b></td>
<td>for <b>4&lt;=x</b>,</td>
</tr>
</tbody></table>

<p>
where <b>pi = 3.1415926535... </b> In this problem, you are asked to compute <b>P(x)</b>
for a given <b>x</b>.
</p>

<h3>Input file specification</h3>
<p>
The input file contains several non-negative integer numbers (less than 30000) each on a separate
line. The last line contains -1 marking the end of the input file.
</p>

<h3>Output file specification</h3>
<p>
For each non-negative real number in the input file, output the corresponding
Pibonacci number. If the Pibonacci number be more than 50 digits long,
divide it on the consecutive lines, outputting 50 digits on each
(the last line may contain less digits).
</p>

<h3>Example</h3>

<b>Input file:</b>
<pre>0
4
11
-1
</pre>

<p>&nbsp;</p>

<b>Output file:</b>
<pre>1
2
20
</pre>