<p>
Elimination of contestants from a live IQ contest on a TV channel is decided in phases.

</p><p>
Initially at phase 0, <span class="MATH"><i>N</i></span>
<tex2html_verbatim_mark> contestants, where <span class="MATH"><i>N</i> = 2<sup>n</sup></span>

<tex2html_verbatim_mark>,
<span class="MATH"><i>n</i> &lt; 10</span>
<tex2html_verbatim_mark>, are selected through a special online IQ contest in which a total of
<span class="MATH"><i>M</i></span>
<tex2html_verbatim_mark> <span class="MATH">(<i>M</i> &gt; <i>N</i>)</span>

<tex2html_verbatim_mark> contestants participate.
The contestants are identified by distinct registration numbers <!-- MATH
 $1, 2, \ldots , M$
 -->
<span class="MATH">1, 2,..., <i>M</i></span>
<tex2html_verbatim_mark>. The
selected contestants are ranked distinctly from 1 to <span class="MATH"><i>N</i></span>
<tex2html_verbatim_mark> according to their
performance in the online contest. They are qualified to participate in the
live contest.

</tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></p><p>
In the <span class="MATH"><i>p</i><sup>th</sup></span>
<tex2html_verbatim_mark> phase, <!-- MATH
 $p=1, 2, \ldots , n, K_{p}$
 -->

<span class="MATH"><i>p</i> = 1, 2,..., <i>n</i>, <i>K</i><sub>p</sub></span>
<tex2html_verbatim_mark>
contestants participate in the live contest, where <!-- MATH
 $K_{p}=2^{n-p+1}$
 -->
<span class="MATH"><i>K</i><sub>p</sub> = 2<sup>n-p+1</sup></span>

<tex2html_verbatim_mark>.
On the basis of response to questions presented during the show, <span class="MATH"><i>K</i><sub>p</sub>/2</span>
<tex2html_verbatim_mark>
of <span class="MATH"><i>K</i><sub>p</sub></span>
<tex2html_verbatim_mark> contestants are ranked distinctly from 1 to <span class="MATH"><i>K</i><sub>p</sub>/2</span>
<tex2html_verbatim_mark>.
These <span class="MATH"><i>K</i><sub>p</sub>/2</span>

<tex2html_verbatim_mark> contestants qualify to participate in the next phase. At
the <span class="MATH"><i>n</i><sup>th</sup></span>
<tex2html_verbatim_mark> phase there are only two contestants and the one selected at
this phase is the winner of the contest.

</tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></p><p>
You are required to write a program that identifies the
winner of the contest, given the following information:

</p><p>

</p><ul>
<li>INFO_1: Registration numbers of <span class="MATH"><i>N</i></span>
<tex2html_verbatim_mark> contestants who are selected through the online IQ
contest, in order of the rank in the online IQ contest, and 

</tex2html_verbatim_mark></li>
<li>INFO_2: A total of <span class="MATH"><i>N</i> - 1</span>
<tex2html_verbatim_mark> qualified contestants in different phases; <span class="MATH"><i>K</i><sub>2</sub></span>
<tex2html_verbatim_mark> in phase 1, <span class="MATH"><i>K</i><sub>3</sub></span>
<tex2html_verbatim_mark>

in phase 2, <span class="MATH">...</span>
<tex2html_verbatim_mark>, and <span class="MATH"><i>K</i><sub>n+1</sub></span>
<tex2html_verbatim_mark> in phase <span class="MATH"><i>n</i></span>
<tex2html_verbatim_mark>. Qualified contestants of
different phases appear in order of phases, i.e., phase 1, phase 2, <span class="MATH">...</span>
<tex2html_verbatim_mark>, phase
<span class="MATH"><i>n</i></span>

<tex2html_verbatim_mark>. Further, qualified contestants in a phase, say phase <span class="MATH"><i>p</i></span>
<tex2html_verbatim_mark>, appear in the order
of the rank in the phase, i.e., the rank in phase <span class="MATH"><i>p</i></span>
<tex2html_verbatim_mark>. A qualified contestant of
a phase, say phase <span class="MATH"><i>p</i></span>
<tex2html_verbatim_mark>, is identified by his/her rank in the previous phase,
i.e., in phase <span class="MATH"><i>p</i> - 1</span>
<tex2html_verbatim_mark>.
</tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></tex2html_verbatim_mark></li>
</ul>

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001001000000000000000">
Input</a>&nbsp;</font>
</h2>

<p>
Input may contain multiple test cases. For each case there are two input lines. 

</p><p>
The first line gives <span class="MATH"><i>N</i></span>
<tex2html_verbatim_mark> integers representing INFO_1
while the second line gives <span class="MATH"><i>N</i> - 1</span>

<tex2html_verbatim_mark> integers representing INFO_2. 

</tex2html_verbatim_mark></tex2html_verbatim_mark></p><p>
In each input line integers are
separated by space. The input terminates with a line containing <tt>0</tt> as input.

</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001002000000000000000">
Output</a>&nbsp;</font>
</h2>

<p>
For each test case there is only one output line. The line
prints the registration number of the winner of the contest.

</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001003000000000000000">
Sample Input</a>&nbsp;</font>
</h2>

<p>
</p><pre>23 18 6 20
4 2 2
29 57 4 33 5 12 16 18
7 1 5 3 2 1 1
0
</pre>  

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001004000000000000000">
Sample Output</a>&nbsp;</font>
</h2>

<p>
</p><pre>18
29
</pre>