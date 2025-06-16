<p>
Rishi loves numbers and number patterns very much.
He is interested in finding OE numbers in a range [a, b].
An OE number is a number whose sum of even digits [0, 2, 4, 6, 8] is greater than sum of odd digits [1, 3, 5, 7, 9].
Help him to count how many OE numbers are in range [a, b] { a and b inclusive }
</p>
<pre>Example: 
  - 4563: O = 5+3   = 8, E = 4+6 = 10, E &gt; O, so 4563 is an OE number
  - 1233, O = 1+3+3 = 7, E = 2,   &nbsp;   &nbsp;E &lt; O, so 1233 is not an OE number
  -   10,&nbsp;O = 1,         E = 0 &nbsp; &nbsp; &nbsp;   E &lt; O, so 10 is not an OE number</pre>

<h3>Input</h3>
<p>
The first line of the input file contains <b>T</b> which denotes the number of Test cases.
The next <b>T</b> lines contains two space seperated integers <b>a</b> and <b>b</b>.</p><p>

</p><p>
1 &lt;= <b>a</b> &lt;= <b>b</b> &lt;=10^8<br>
<b>T</b> &lt;= 35.
</p>

<h3>Output</h3>
<p>
Print the number of OE numbers in range [<b>a</b>, <b>b</b>] {one number per line}
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 1
2 10
1 100000000

<strong>Output:</strong>
0
4
38379932</pre>