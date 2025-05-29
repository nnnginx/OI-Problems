<p>Borussia Dortmund is a famous football ( soccer ) club from Germany.  Apart from their fast style of playing, the thing that makes them unique  is the hard to pronounce names of their players ( błaszczykowski ,  papastathopoulos , großkreutz etc. ).<br><br>The team's coach is your  friend. He is in a dilemma as he can't decide how to make it easier to  call the players by name, during practice sessions. So, you advised him  to assign easy names to his players. A name is easy to him if</p>
<ol>
<li>It consists of only lowercase english letters.</li>
<li>It's length is exactly <strong><em>N</em></strong>.</li>
<li>It contains <strong>exactly <em>K</em></strong> different letters from the <strong><em>26</em></strong> letters of english alphabet.</li>
<li>At least one of its <strong>proper</strong> prefixes matches with its <strong>proper</strong> suffix of same length.</li>
</ol>
<p>Given, <strong><em>N</em></strong> and <strong><em>K</em></strong> you have to tell him the number of easy names he can choose from modulo <strong><em>(10^9+9)</em></strong>.</p>
<p><strong>Note :</strong> A prefix <strong><em>P</em></strong> of a name <strong><em>W</em></strong> is proper if, <strong><em>P</em>&nbsp;≠ <em>W</em></strong>. Similarly, a suffix <strong><em>S</em></strong> of a name <strong><em>W</em></strong> is proper if, <strong><em>S</em>&nbsp;≠ <em>W</em></strong>.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input will contain <strong><em>T</em></strong> ( the number of testcases ).<br>Each of the next <strong><em>T</em></strong> lines will contain two space separated integers <strong><em>N</em></strong> and <strong><em>K</em></strong>.</p>
<h3>Output</h3>
<p>For each testcase, output the number of ways the coach can assign names to his players modulo <strong><em>(10^9+9)</em></strong>.</p>
<h3>Constraints</h3>
<p><strong><em>1&nbsp;≤ T&nbsp;≤ 10<sup>5</sup>&nbsp; <br>1&nbsp;≤ N&nbsp;≤ 10<sup>5</sup>&nbsp;&nbsp;&nbsp; <br>1&nbsp;≤ K&nbsp;≤ 26</em></strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8<br>1 1<br>2 1<br>4 2<br>2 2<br>5 1<br>3 2<br>6 2<br>1 3

<strong>Output:</strong>
0<br>26<br>2600<br>0<br>26<br>650<br>13650<br>0</pre>