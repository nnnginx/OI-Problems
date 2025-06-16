<p>
Let <i> K</i> be a decimal digit different from <i>0</i>. We say that an
arithmetic expression is a <b>K-representation of the integer X</b>
if a value
of this expression is X and if it contains only numbers composed of a
digit K.
(All the numbers are of course decimal). The following arithmetical
operations are allowed in the expression: addition, subtraction,
multiplication and division. Round brackets are
allowed too. Division may appear only when a dividend is a multiple of
a
divisor.
</p>

<h3>Example</h3>
<p>
Each of the following expressions is the 5-representation of the number 12:
</p>
<ul>
 <li>5+5+(5:5)+(5:5)
 </li><li>(5+(5))+5:5+5:5
 </li><li>55:5+5:5
 </li><li>(55+5):5
</li></ul>
<p>
The<b> length</b> of the <i>K</i>-representation is the number of occurrences of
digit <i>K</i> in the expression. In the example above the first two representations have the length 6, the third - 5, and the forth - 4.
</p>

<h3>Task</h3>
<p>
Write a program which:&nbsp;
</p>
<ul>
 <li>reads the digit <i> K</i> and the series of numbers from the standard input,
 </li><li>verifies for each number from the series, whether it has a <i>K</i>-representation
  of length at most 8, and if it does, then the program finds the minimal length of this representation,
 </li><li>writes results to the standard output.&nbsp; 
</li></ul>

<h3>Input</h3>
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
The first line of each test case contains digit <i>K</i>, <i> K</i> is en element of
{<i>1,...,9</i>}. The second line
contains number n, <i> 1&lt;=n&lt;=10</i>. In the following <i> n</i> lines there is the series  of natural numbers
<i> a<sub>1</sub>,...,a<sub>n</sub></i>, <i> 
1&lt;=a<sub>i</sub>&lt;=32000</i> (for <i>i=1,..,n</i>), one number in each line.&nbsp; 
</p>

<h3>Output</h3>
<p>
The output for each test case composes of <i> n</i> lines. The <i>i-</i>th line should
contain:&nbsp;
</p>
<ul>
 <li>exactly one number which is the minimal length of <i>K</i>-representation of a<sub><i>i</i></sub>,
  assuming that such a representation of length not grater then 8 exists,
 </li><li>one word NO, if the minimal length of the <i>K</i>-representation of the number
  <i> a</i><sub><i>i</i></sub>
  is grater than 8.&nbsp;
</li></ul>

<h3>Example</h3>

<pre><b>Sample input:</b>
1
5
2
12
31168

<b>Sample output</b>
4
NO
</pre>