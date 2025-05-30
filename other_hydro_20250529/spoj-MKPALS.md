<p>A <i>palindrome</i> is a sequence that is the same when read forward or backward. For example, ��pop�� is a
palindrome, as are ��Poor Dan is in a droop�� (ignoring spaces and case), and ��12321��.

</p><p></p><p>
In this problem, you are to find the ��cheapest�� way to transform a sequence of decimal digits into a
palindrome. There are only two types of modifications you may make to the sequence, but each of these
may be repeated as many times as necessary. You may delete a digit from either end of the sequence, or
you may add a digit to either end of the sequence. Each of these operations incurs a ��cost�� of 1. For each
input sequence, determine the smallest cost of transforming the sequence into a palindrome, and the length
of the resulting palindrome. If two palindromes can be produced with the same cost, the length of the
longer palindrome (the one with more digits) is to be reported.

</p><p></p><p>
For example, suppose the initial sequence was ��911��. This can be transformed into a palindrome by deleting
the leading ��9�� (yielding ��11��) or by adding an additional ��9�� to the right end of the sequence (yielding
��9119��). Since both of these transformations have a cost of 1, and the second transformation yields a
longer palindrome, it is this one which would be reported as your result.

</p><p></p><p>
Note that the particular palindrome produced by the cheapest sequence of transformations is not
necessarily unique, but since you are not required to report the resulting palindrome, any of these will
suffice.

</p><h3>Input</h3>
<p>There will be multiple cases to consider. Each case has a single line of input that contains one or more
decimal digits followed by the end of line. The maximum number of digits in a sequence will be 6. The last
case is followed by an empty line (that is, only an end of line).

</p><h3>Output</h3>
<p>For each input case, display the case number (1, 2, ��), the input sequence, the cost of the cheapest
transformation, and the length of the resulting palindrome. Your output should follow the format shown in
the examples below.

</p><h3>Example</h3>

<pre><b>Input:</b>
911
9118
11234
&lt;-- This line is blank

<b>Output:</b>
Case 1, sequence = 911, cost = 1, length = 4
Case 2, sequence = 9118, cost = 2, length = 4
Case 3, sequence = 11234, cost = 3, length = 8
</pre>