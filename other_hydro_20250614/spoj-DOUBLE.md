<p>Some numbers have a curious property: when rotating the number to the right,
the new number is the double of the original. Rotating the number to
the right means choosing the last digit and moving it to the beginning of the number,
as the leftmost digit. For example, the number 421052631578947368 when
rotated to the right gives 842105263157894736, which is the double
of the original. These numbers are expressed in the decimal system. In any
numeral system such numbers exist, for example, in the binary (base 2)
numeral system, numbers 01 and 0101 have this property.
Note that leading zeros are required in this case.

</p><p>Write a program that, for any given base B (2 &lt;= B &lt;= 250), finds the
smallest number in that numeral system which has this property. Try not to
precompute the numbers, the solution is very easy and pretty.

</p><h3>Input</h3>

<p>The input consists of several test cases. The first line contains an
integer T (T &lt;= 20), the number of test cases. The following T lines
contain one number B, each.

</p><h3>Output</h3>

<p>For each number B, output one or more numbers separated by a blank
space that represent the digits in base B (written as decimal numbers) of the smallest number which has
this property.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
2
10
35
<b>Output:</b>
0 1
0 5 2 6 3 1 5 7 8 9 4 7 3 6 8 4 2 1
11 23
</pre>

<h3>Output explanation</h3>
<pre>In  example #1
The initial number (when converted to decimal system):
0 * 2^1 + 1 * 2^0 = 1 
After applying the rotation:
1 * 2^1 + 0 * 2^0  = 2.

In example #3
The initial number (when converted to decimal system):
11 * 35^1 + 23 * 35^0  =  408
After applying the rotation:
23 * 35^1 + 11 * 35^0  = 816.
</pre>