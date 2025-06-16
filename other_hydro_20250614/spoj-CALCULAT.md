<p>Dan likes playing with his pocket calculator during those long, boring math classes. Just now the teacher started to talk about the factorial function. </p>

<p><b>N</b> factorial, denoted by <b>N!</b>, is the product of all the integers between 1 and <b>N</b>, inclusive. For example 6! = 6*5*4*3*2*1 = 720. </p>

<p>Dan took out his calculator out of his pocket to play around with this new function. Unfortunately his calculator quickly ran out of digits and only showed overflow errors. Soon, Dan realized that the factorial function grows very quickly. Still, he would like to know at least some of its digits. </p>

<h3>Problem specification</h3>
<p>Given three positive integers <b>N</b>(1&lt;= <b>N</b> &lt;=10<sup>8</sup>), <b>K</b>(1&lt;= <b>K</b> &lt;=50), <b>L</b>(1&lt;= <b>L</b> &lt;=100), compute the first <b>K</b> digits and the last <b>L</b> digits of <b>N</b> factorial. </p>

<h3>Input specification</h3>
<p>The first line of the input file contains an integer <b>T</b> specifying the number of test cases. Each test case is preceded by a blank line. </p>

<p>Each test case consists of one line containing three positive integers <b>N</b>, <b>K</b> and <b>L</b> separated by single spaces. Neither <b>K</b> nor <b>L</b> will exceed the number of digits in <b>N!</b>. 

</p><h3>Output specification</h3>
<p>For each test case output one line containing two strings <b>A</b> and <b>B</b> separated by a single space. Here, <b>A</b> is the string composed of the first <b>K</b> digits of <b>N!</b> and <b>B</b> is the string composed of the last <b>L</b> digits of <b>N!</b>. 

</p><h3>Example</h3>
<pre><b>Input:</b>
3

6 2 1

10 3 2

8 5 5

<b>Output:</b>
72 0
362 00
40320 40320
</pre>
<b>Note : for all test cases whose N&gt;=100, its K&lt;=15.</b>