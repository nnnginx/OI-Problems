<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">string clockwise on a ring, with the first</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">character following on the last, starting at</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">any character position and moving clock-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">wise on the ring until the character pre-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">ceeding the starting character is reached.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A string is a necklace if it is the lexico-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">graphically smallest among all its cyclic</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">rotations. For instance, for the string 01011 the cyclic rotations are</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">(10110,01101,11010,10101,01011), and furthermore 01011 is the smallest</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">string and hence, a necklace.</div>
<p>The set of cyclic rotations of a string are&nbsp;the strings obtained by embedding the&nbsp;string clockwise on a ring, with the first&nbsp;character following on the last, starting at&nbsp;any character position and moving clockwise on the ring until the character preceeding the starting character is reached.&nbsp;A string is a necklace if it is the lexicographically smallest among all its cyclic&nbsp;rotations. For instance, for the string 01011 the cyclic rotations are&nbsp;(10110,01101,11010,10101,01011), and furthermore 01011 is the smallest&nbsp;string and hence, a necklace.</p>
<div>
<div>Any string S can be written in a unique way as a concatenation S =&nbsp;T1 T2 . . . Tk of necklaces Ti such that Ti+1 &lt; Ti for all i = 1, . . . , k − 1, and&nbsp;Ti Ti+1 is not a necklace for any i = 1, . . . , k − 1. This representation is&nbsp;called the necklace decomposition of the string S, and your task is to find&nbsp;it.</div>
</div>
<div>
<div>The relation &lt; on two strings is the lexicographical order and has the&nbsp;usual interpretation: A &lt; B if A is a proper prefix of B or if A is equal to&nbsp;B in the first j − 1 positions but smaller in the jth position for some j. For&nbsp;instance, 001 &lt; 0010 and 1101011 &lt; 1101100.</div>
</div>
<h3>Input</h3>
<p>On the first line of the input is a single positive integer n, telling the&nbsp;number of test scenarios to follow. Each scenario consists of one line&nbsp;containing a non-empty string of zeros and ones of length at most 100.</p>
<h3>Output</h3>
<p>For each scenario, output one line containing the necklace decomposition&nbsp;of the string. The necklaces should be written as ’(’ necklace ’)’.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
0
0101
0001
0010
11101111011

<strong>Output:</strong>
(0)
(0101)
(0001)
(001)(0)
(111)(01111)(011)</pre>