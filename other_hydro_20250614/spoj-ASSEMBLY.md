<p>The last worker in a production line at the factory of Automated Composed Machinery is worried. She knows that her job hangs in the balance unless her productivity increases. Her work consists of assembling a set of pieces in a given sequence, but the time spent on assembling pieces <em>a</em> and <em>b</em> and then <em>c</em> may not the same as that on assembling pieces <em>b</em> and <em>c</em>, and then assembling <em>a</em> with the resulting component. Only two consecutive pieces may be assembled at a time, and once they are assembled they behave as another piece in terms of the time needed for further assembly.</p>
<p>In order to aid her, you need to find the optimal way to assemble all components. The input to your program will be a set of symbols representing (types of) pieces, and a so-called assembly table representing the time it takes to assemble them, as well as the type of the resulting component. For instance, we may have two symbols {<em>a</em>,<em>b</em>}, and the following table:</p>
<div class="center">
<table border="1" cellspacing="0" cellpadding="1">
<tbody>
<tr>
<td align="left">&nbsp;</td>
<td align="left"><em>a</em></td>
<td align="left"><em>b</em></td>
</tr>
<tr>
<td align="left"><em>a</em></td>
<td align="left">3<code>-</code><em>b</em></td>
<td align="left">5<code>-</code><em>b</em></td>
</tr>
<tr>
<td align="left"><em>b</em></td>
<td align="left">6<code>-</code><em>a</em></td>
<td align="left">2<code>-</code><em>b</em></td>
</tr>
</tbody>
</table>
</div>
<p>This means, for example, that two pieces of type <em>a</em> and <em>a</em> may be assembled in 3 minutes, and the result is a component of type <em>b</em>, in that the time required to assemble it again with another piece of, say, type <em>a</em> is 6 minutes, and so on. Note that the table is not symmetric, i.e. assembling <em>b</em> and <em>a</em> may be more time-consuming than <em>a</em> and <em>b</em>.</p>
<p>For a sequence of components labelled <em>aba</em>, the two possible solutions are:</p>
<ul class="itemize">
<li class="li-itemize"> (<em>ab</em>)<em>a</em> = <em>ba</em> = <em>a</em> with time <em>time</em>(<em>ab</em>) + <em>time</em>(<em>ba</em>) = 5+6 = 11. </li>
<li class="li-itemize"><em>a</em>(<em>ba</em>) = <em>aa</em> = <em>b</em> with time <em>time</em>(<em>ba</em>) + <em>time</em>(<em>aa</em>) = 6+3 = 9. </li>
</ul>
<p>So the result for this case would be a piece of type <em>b</em> in 9 minutes (denoted 9<code>-</code><em>b</em>).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of several test cases. Each test case begins with a line containing a natural number <em>k</em> (1 �� <em>k</em> �� 26), followed by a line with <em>k</em> symbols (characters in <code>[a-z]</code>) separated by spaces. The following <em>k</em> lines contain the assembly table: the <em>i</em>-th line has <em>k</em> pairs of the form <em>time</em><code>-</code><em>result</em>, where <em>time</em> is an integer between 0 and 1&nbsp;000&nbsp;000 inclusive, and <em>result</em> a symbol belonging to the preceding set. The <em>j</em>-th pair in the <em>i</em>-th line represents the time to compose pieces of types represented by the <em>i</em>-th and <em>j</em>-th symbols, along with the type of the resulting piece. After the table, a line with an integer <em>n</em> indicates the number of lines that follow, each line being a string of at most 200 symbols. Each of these lines is a sequence of components that need to be assembled together in the right order.</p>
<p>The input will finish with a line containing <tt>0</tt>, which should not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each test case, print <em>n</em> lines, each with an integer <em>time</em> and a symbol <em>result</em> in the format <em>time</em><code>-</code><em>result</em>. Each line represents the minimum time and the type of the resulting piece for the corresponding case in the input. In case of a tie among several possible results with the same minimum time, choose from among those the piece whose type letter appears first in the line that contained the <em>k</em> symbols at the beginning of the test case. (For example, if that line was <em>a</em>&nbsp; <em>c</em>&nbsp; <em>b</em> and both <em>c</em> and <em>b</em> can be obtained with minimum cost 5, print 5<code>-</code><em>c</em>).</p>
<p>There must be an empty line between the output of different test cases. <br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">2
a b
3-b 5-b
6-a 2-b
2
aba
bba
2
m e
5-e 4-m
3-e 4-m
1
eme
0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">9-b
8-a

7-m
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Enrique Mart��n Mart��n</em></blockquote>