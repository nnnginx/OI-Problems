<p>Billy Jean loves collecting frogs.&nbsp; Recently, she developed the sport of frog wrestling.&nbsp; Now she wants to rank her frogs by their wrestling prowess.</p>
<p>Billy Jean has made a algorithm for sorting her frogs.</p>
<ol>
<li>She arranges N cages, numbered 1,2,...N, each with one frog.</li>
<li>For each pair of cages in a specified, pre-determined list of K pairs of cages,<ol>
<li>she removes the frogs from the two cages,</li>
<li>has the frogs wrestle,</li>
<li>puts the winner in the higher-numbered cage, and</li>
<li>puts the loser in the lower-numbered cage.</li>
</ol></li>
</ol>
<p>When she is finished, she hopes to have all her frogs sorted from worst to best in the cages 1 to N.&nbsp; Will her algorithm work regardless of the initial order of the frogs?</p>
<p>Note:</p>
<ul>
<li>Assume that a strict ordering by wrestling ability is possible.</li>
<li>Billy Jean isn't the sharpest tool in the shed.&nbsp; Sometimes she has written the same two numbers for a pair.&nbsp; In this case, that frog is simply taken out and then put back.</li>
</ul>
<h3>Constraints</h3>
<p>1&lt;=N&lt;=20</p>
<p>1&lt;=K&lt;=1000</p>
<h3>Input</h3>
<p>The first line is the number of test cases.&nbsp; Each test cases is preceded by a blank line.</p>
<p>The first line of each test case is N.&nbsp; The next line is K.&nbsp; The next K lines are the pairs, separated by a single space.</p>
<h3>Output</h3>
<p>On separate lines, output whether Billy Jean's algorithm is correct.&nbsp; Output "YES" (without quotes) if it is or "NO" (without quotes) if it is not.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4<br><br>2<br>1<br>2 1<br><br>2<br>1<br>1 1<br><br>1<br>1<br>1 1<br><br>4<br>5<br>1 2<br>3 4<br>1 3<br>2 4<br>2 3<br><br><strong>Output:</strong>
YES<br>NO<br>YES<br>YES</pre>