<p>
One part of the new WAP portal is also a&nbsp;calculator computing expressions
with very long numbers. To make the output look better, the result is
formated the same way as is it usually used with manual calculations.

</p><p>
Your task is to write the core part of this calculator. Given two numbers and
the requested operation, you are to compute the result and print it in the
form specified below. With addition and subtraction, the numbers are written
below each other. Multiplication is a&nbsp;little bit more complex: first of all, we
make a&nbsp;partial result for every digit of one of the numbers, and then sum the
results together.

</p><p>
</p><h3>Input</h3>

<p>

There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 1000). It stands
for the number of expressions to follow. Each expression consists of a&nbsp;single
line containing a&nbsp;positive integer number, an&nbsp;operator (one of <tt>+</tt>,
<tt>-</tt> and <tt>*</tt>) and the second positive integer number. Every number has
at most 500&nbsp;digits. There are no spaces on the line. If the operation is
subtraction, the second number is always lower than the first one. No number
will begin with zero.

</p><p>

</p><h3>Output</h3>

<p>
For each expression, print two lines with two given numbers, the second
number below the first one, last digits (representing unities) must be
aligned in the same column. Put the operator right in front of the first
digit of the second number. After the second number, there must be
a&nbsp;horizontal line made of dashes (<tt>-</tt>).

</p><p>
For each addition or subtraction, put the result right below the horizontal
line, with last digit aligned to the last digit of both operands.

</p><p>
For each multiplication, multiply the first number by each digit of the
second number. Put the partial results one below the other, starting with the
product of the last digit of the second number. Each partial result should be
aligned with the corresponding digit.
That means the last digit of the partial product must be in the same column
as the digit of the second number. No product may begin with any additional
zeros. If a&nbsp;particular digit is zero, the product has exactly one digit --
zero. If the second number has more than one digit, print another horizontal
line under the partial results, and then print the sum of them.

</p><p>
There must be minimal number of spaces on the beginning of lines, with
respect to other constraints. The horizontal line is always as long as
necessary to reach the left and right end of both numbers (and operators)
directly below and above it. That means it begins in the same column where the
leftmost digit or operator of that two lines (one below and one above) is. It
ends in the column where is the rightmost digit of that two numbers. The line
can be neither longer nor shorter than specified.

</p><p>
Print one blank line after each test case, including the last one.

</p><h3>Example</h3>

<p>Sample Input:</p><pre><tt>4
12345+67890
324-111
325*4405
1234*4
</tt>
</pre>

<p>Sample Output:</p><pre><tt> 12345
+67890
------
 80235

 324
-111
----
 213

    325
  *4405
  -----
   1625
     0
 1300
1300
-------
1431625

1234
  *4
----
4936</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages.</b>