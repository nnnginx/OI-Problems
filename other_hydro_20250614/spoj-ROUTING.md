<p>You work as an engineer for the <em>Inane Collaboration for Performance Computing</em>, where you are in charge of designing an intercommunication network for their computers. The network is arranged as a rectangular array of 2<em>n</em>−1 rows, each having 2<sup><em>n</em> − 1</sup> switches. A switch is a device with two input wires, <em>X</em> and <em>Y</em>, and two output wires, <em>X</em>′ and <em>Y</em>′. If the switch is off, data from input <em>X</em> will be relayed to output <em>X</em>′, and data from <em>Y</em> to <em>Y</em>′. If it is on, <em>X</em> will be connected to <em>Y</em>′ and <em>Y</em> to <em>X</em>′. Additionally, there are 2<sup><em>n</em></sup> computers in the topmost and bottommost rows, and messages need to be sent between pairs of them. Notice that data from two different sources cannot share a wire but, of course, both pieces of data can be routed through the same switch on different inputs.</p>
<p>You have come to the conclusion that the network that best suits your purposes has the Beneš topology. A 1-Beneš network is just a switch. For <em>n</em> &gt; 1, a <em>n</em>-Beneš network can be constructed recursively as follows:</p>
<ul class="itemize">
<li class="li-itemize">In the first (top) row there are 2<sup><em>n</em> − 1</sup> switches such that switch <em>j</em> (0 ≤ <em>j</em> &lt; 2<sup><em>n</em>−1</sup>) has data inputs from computers 2<em>j</em> and 2<em>j</em> + 1 (we label the computers in the topmost and bottommost rows with integers between 0 and 2<sup><em>n</em></sup> − 1, inclusive, from left to right).</li>
<li class="li-itemize">Then a <em>perfect shuffle</em> permutation is applied to the output wires between the first and the second rows of switches, meaning that output number <em>j</em> in a row is connected to input number <em>j</em>′ in the next row, where <em>j</em>′ is obtained by rotating the n-bit pattern representing <em>j</em> in binary one bit to the right (again, inputs and outputs are numbered from left to right).</li>
<li class="li-itemize">If <em>n</em> &gt; 2, the next rows of switches, up to (and including) the last-but-one, form two (<em>n</em>−1)-Beneš subnetworks, one on the left side and the other on the right side.</li>
<li class="li-itemize">Finally, the <em>inverse</em> shuffle permutation is applied to the outputs and a last row of switches is added.</li>
</ul>
<blockquote class="figure">
<div class="center">
<div class="center">
<hr size="2">
</div>
<a name="benes"></a> <img src="../../../content/elhipercubo:redbenes.jpg" alt="" width="100" height="200"> &nbsp;&nbsp;&nbsp;  <a name="sample"></a> <img src="../../../content/elhipercubo:redbenes_color.jpg" alt="" width="100" height="200">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">3-Benes network</td>
</tr>
</tbody>
</table>
</div>
<div class="center">
<hr size="2">
</div>
</div>
</blockquote>
<p>For example, the figure on the left shows the Beneš network for <em>n</em>=3 ( squares represent switches; computers in the top and bottom rows are not drawn, but assigned with integers from 0 to 7). The figure on the right&nbsp;shows a possible state of the switches; squares where two of the lines cross are switches that have been turned on. You may verify that this state allows us to simultaneously establish communication paths from computers 0, 1, 2, 3, 4, 5, 6, 7 at the bottom to 3, 7, 4, 0, 2, 6, 1, 5 at the top, respectively.</p>
<p>You are given a set of pairs (<em>a</em>, <em>b</em>) of computers to connect simultaneously (where <em>a</em> is a computer in the bottom row and <em>b</em> a computer in the top row) by means of wire-disjoint paths, and you are to find how to select the state of all switches so that this can be accomplished.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each test case is an integer <em>n</em> (1 ≤ <em>n</em> ≤ 13), meaning that you have 2<sup><em>n</em></sup> pairs of computers to connect, as described above. A line with <em>n</em> = 0 marks the end of the input and should not be processed.</p>
<p>Each line with <em>n</em> &gt; 0 will be followed by another line containing 2<sup><em>n</em></sup> integers. The <em>i</em>-th integer (0 ≤ <em>i</em> &lt; 2<sup><em>n</em></sup>) will be the computer in the topmost row that the <em>i</em>-th computer in the bottommost row needs to communicate with.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>The output for each case should have 2<em>n</em>−1 lines, each containing a binary string of length 2<sup><em>n</em>−1</sup> indicating, for each switch, whether it must be turned on (1) or off (0).</p>
<p>The input given will always have at least one solution. In case of several solutions, return the lexicographically smallest one. That is, the string in the top row must be lexicographically smallest; in case of a tie, the string in the second row must be lexicographically smallest, and so on.</p>
<p>Outputs for different test cases should be separated by a blank line.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2
3 2 1 0
3
3 7 4 0 2 6 1 5
0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">00
11
11

0011
0000
0110
1111
1101
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David García Soriano</em></blockquote>