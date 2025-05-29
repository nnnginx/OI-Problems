<p>The digit-product of a positive integer is the product of the number's decimal digits. For example, the digit-product of 2612 is 2 ¡¤ 6 ¡¤ 1 ¡¤ 2 = 24.</p>

<p>The self-product of a number is the product of the number and its digit-product. For example, the self-product of 2612 is 2612 ¡¤ 24 = 62688.</p>

<p>Write a program that, given two positive integers A and B (1 ¡Ü A ¡Ü B &lt; 10<sup>18</sup>), calculates the number of positive integers whose self-product is between A and B, inclusive.</p>

<h3>Input</h3>
<p>The first line of input contains the integer T (1 ¡Ü T ¡Ü 20). The next T lines each contain a pair of integers A and B.</p>

<h3>Output</h3>
<p>For each test case, print a line with the number of positive integers whose self-product is between A and B.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
20 30
145 192
2224222 2224222

<b>Output:</b>
2
4
1
</pre>

<p>For the second example, the self-products of the numbers 19, 24, 32, and 41 are 171, 192, 192 and 164, respectively.</p>