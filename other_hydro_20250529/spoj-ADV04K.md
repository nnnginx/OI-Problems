<p>Once little Petya was learning positional numeral systems. Using such systems the numbers are represented as the sequence of digits</p>
<div align="center"><table class="display dcenter"><tbody><tr valign="middle"><td class="dcell">
</td><td class="dcell"><table border="0" cellspacing="1" cellpadding="0"><tbody><tr><td class="hbar"></td></tr>
<tr><td align="center" nowrap=""><i>a</i><sub><i>n</i></sub>&nbsp;<i>a</i><sub><i>n</i>−1</sub>&nbsp;…&nbsp;<i>a</i><sub>2</sub>&nbsp;<i>a</i><sub>1</sub>&nbsp;<i>a</i><sub>0</sub></td></tr>
</tbody></table></td><td class="dcell">&nbsp;=&nbsp;</td><td class="dcell"><table class="display"><tbody><tr><td class="dcell" align="center"><i>n</i></td></tr>
<tr><td class="dcell" align="center"><font size="6">∑</font></td></tr>
<tr><td class="dcell" align="center"><i>k</i>=0</td></tr>
</tbody></table></td><td class="dcell">&nbsp;<i>a</i><sub><i>k</i></sub>&nbsp;<i>b</i><sup><i>k</i></sup>,
</td></tr>
</tbody></table></div>
<p>where b is the base of the numeral system, and 0 &lt;= a<sub>k</sub> &lt; b. Petya was dissapointed that one can represent only non-negative numbers this way. But then he found out that there are systems with negative base such as negabinary system in which b = −2, a<sub>k</sub> ∈ {0, 1}. One can represent any integer in this system for example 1110<sub>−2</sub> = −6. Moving the idea further Petya came up with his own base b using which he could represent even more numbers given a<sub>k</sub> ∈ {0, 1}. 
However performing arithmetic operations in this non-standard system turned to be rather difficult. Help Petya implement a calculator for his numeral system.

</p><h3>Input</h3>
<p>The first line of input is number T - the amount of test cases. Next T lines contain the description of arithmetic expression consisting of two operands and an opertaion separated with spaces. Both operands consist of one ‘0’ and ‘1’ digits and have the length of no more than 100. Operation is one of ‘+’, ‘-’ or ‘*’.

</p><h3>Constraints</h3>
<p>1 &lt;= T &lt;= 1000

</p><h3>Output</h3>
<p>For each test case output a number which is the result of evaluating the given expression.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
11 - 11
1 + 1
1100 * 1100
1101 - 11
111 * 1

<b>Output:</b>
0
1100
111010000
111010110
111

</pre>