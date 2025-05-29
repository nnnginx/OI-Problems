<p>Binary numbers form the principal basis of computer science. Most of you have heard of other
systems, such as ternary, octal, or hexadecimal. You probably know how to use these systems
and how to convert numbers between them. But did you know that the system base (radix)
could also be negative. One assistant professor at the Czech Technical University has recently
met negabinary numbers and other systems with a negative base. Will you help him to convert
numbers to and from these systems.

</p><p>A number N written in the system with a positive base R will always appear as a string of
digits between 0 and R - 1, inclusive. A digit at the position P (positions are counted from
right to left and starting with zero) represents a value of R^P. This means the value of the 
digit is multiplied by R^P and values of all positions are summed together. 
For example, if we use the octal system (radix R = 8), a number written as 17024 has the following value:
</p><p>1.8^4 + 7.8^3 + 0.8^2 + 2.8^1 + 4.8^0 = 1.4096 + 7.512 + 2.8+4.1 = 7700

</p><p>With a negative radix -R, the principle remains the same: each digit will have a value of (-R)^P.
For example, a negaoctal (radix R = -8) number 17024 counts as:
</p><p>1.(-8)^4 + 7.(-8)^3 + 0.(-8)^2 + 2.(-8)^1 + 4.(-8)^0 = 1.4096 - 7.512 - 2.8+4.1 = 500

</p><p>One big advantage of systems with a negative base is that we do not need a minus sign to express
negative numbers. A couple of examples for the negabinary system (R = -2):
</p><p>
</p><table border="1">
 <tbody><tr><td>decimal</td>
     <td>negabinary</td>
     <td>decimal</td>
     <td>negabinary</td>
     <td>decimal</td>
     <td>negabinary</td>
 </tr>
 <tr>
     <td>-10<br>-9<br>-8<br>-7<br>-6<br>-5<br>-4</td>
     <td>1010<br>1011<br>1000<br>1001<br>1110<br>1111<br>1100</td>
     <td>-3<br>-2<br>-1<br>0<br>1<br>2<br>3</td>
     <td>1101<br>10<br>11<br>0<br>1<br>110<br>111</td>
     <td>4<br>5<br>6<br>7<br>8<br>9<br>10</td>
     <td>100<br>101<br>11010<br>11011<br>11000<br>11001<br>11110</td>
 </tr>
</tbody></table>

<p>You may notice that the negabinary representation of any integer number is unique, if no "leading
zeros" are allowed. The only number that can start with the digit "0", is the zero itself.

</p><h3>Input</h3>
<p>The input will contain several conversions, each of them specified on one line. A conversion
from the decimal system to some negative-base system will start with a lowercase word "to"
followed by a minus sign (with no space before it), the requested base (radix) R, one space, and
a decimal number N.

</p><p>A conversion to the decimal system will start with a lowercase word "from", followed by a minus
sign, radix R, one space, and a number written in the system with a base of -R.

</p><p>The input will be terminated by a line containing a lowercase word "end". All numbers will
satisfy the following conditions: 2 &lt;= R &lt;= 10, -1 000 000 &lt;= N &lt;= 1 000 000 (decimal).

</p><h3>Output</h3>
<p>For each conversion, print one number on a separate line. If the input used a decimal format,
output the same number written in the system with a base -R. If the input contained such
a number, output its decimal value.

</p><p>Both input and output numbers must not contain any leading zeros. The minus sign "-"may
only be present with negative numbers written in the decimal system. Any non-negative number
or a number written in a negative-base system must not start with it.


</p><h3>Example</h3>
<pre><b>Input</b>
to-2 10
from-2 1010
to-10 10
to-10 -10
from-10 10
end

<b>Output</b>
11110
-10
190
10
-10

</pre>