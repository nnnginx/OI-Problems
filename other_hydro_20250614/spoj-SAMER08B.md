<p>What do you get if you multiply 6 by 9? The answer, of course, is 42, but only if you do the calculations in base 13.</p>
<p>Given an integer <em>B</em> �� 2, the <em>base <em>B</em> numbering system</em> is a manner of writing integers using only digits between 0 and <em>B</em> -1, inclusive. In a number written in base <em>B</em>, the rightmost digit has its value multiplied by 1, the second rightmost digit has its value multiplied by <em>B</em>, the third rightmost digit has its value multiplied by <em>B</em><sup>2</sup>, and so on.</p>
<p>Some equations are true or false depending on the base they are considered in. The equation 2+2=4, for instance, is true for any <em>B</em> �� 5 - it does not hold in base 4, for instance, since there is no digit '4' in base 4. On the other hand, an equation like 2+2=5 is never true.</p>
<p>Write a program that given an equation determines for which bases it holds.</p>
<h3>Input</h3>
<p>Each line of the input contains a test case; each test case is an equation of the form "<tt>EXPR=EXPR</tt>", where both  "<tt>EXPR</tt>" are arithmetic expressions with at most 17 characters.</p>
<p>All expressions are valid, and contain only the characters '<tt>+</tt>', '<tt>*</tt>' and the digits from '<tt>0</tt>' to '<tt>9</tt>'. No expressions contain leading plus signs, and no numbers in it have leading zeros.</p>
<p>The end of input is indicated by a line containing only "<tt>=</tt>".</p>
<h3>Output</h3>
<p>For each test case in the input your program should produce a single line in the output, indicating for which bases the given equation holds.</p>
<p>If the expression is true for infinitely many bases, print  "<tt>B+</tt>", where <em>B</em> is the first base for which the equation holds.</p>
<p>If the expression is valid only for a finite set of bases, print them in ascending order, separated by single spaces.</p>
<p>If the expression is not true in any base, print the character '<tt>*</tt>'.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6*9=42
10000+3*5*334=3*5000+10+0
2+2=3
2+2=4
0*0=0
=


<strong>Output:</strong>
13
6 10
*
5+
2+

</pre>