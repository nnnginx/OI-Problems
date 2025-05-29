<p>For a directed graph <em>G</em> where any vertex <em>v</em> has two  weights <em>A<sub>v</sub></em> and <em>B<sub>v</sub></em>, we call <em>A<sub>u</sub></em>+<em>B<sub>v</sub></em> the weight of a edge (<em>u</em>,<em>v</em>). Let <em>MaxEdge</em>(<em>G</em>)  be the maximum weight of the edges of <em>G</em>.</p>
<p>Given a permutation <em>P</em> on 1..<em>n</em>, we can derive a directed graph <em>G</em>=(<em>V</em>,<em>E</em>)  where <em>V</em>={1,..,<em>n</em>} and (<em>u</em>,<em>v</em>) in <em>E</em> iff  <em>P</em>(<em>u</em>)=<em>v</em>. Your task is to compute <em>MaxEdge</em>(<em>P<sup>k</sup></em>)  for every <em>k</em> in 0..<em>q</em>-1.</p>
<h3>Input</h3>
<p>The first line contains a positive integer <em>n</em>.<br>The second line  contains <em>n</em> integers in {1,..,<em>n</em>}, denoting the permutation <em>P</em>.<br>The  third and the fourth line both contain <em>n</em> natural numbers, <em>A</em><sub>1</sub>,..,<em>A<sub>n</sub></em> and <em>B</em><sub>1</sub>,..,<em>B<sub>n</sub></em> respectively.<br>The fifth line contains a  positive integer <em>q</em>.</p>
<h3>Output</h3>
<p>The only one line contains <em>q</em> integers <em>MaxEdge</em>(<em>P</em><sup>0</sup>),..,<em>MaxEdge</em>(<em>P<sup>q</sup></em><sup>-1</sup>), separated by a single space.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>3 2 1<br>0 1 2<br>2 2 0<br>5<br><br><strong>Output:</strong><br>3 4 3 4 3<br></pre>
<h3>Constraint</h3>
<p><em>n</em> &lt;= 66000<em><br>A<sub>i</sub>, </em><em>B<sub>i</sub></em> &lt;= 16<br><em>q</em> &lt;= 10<sup>6</sup><em><br></em></p>
<h3>Notice</h3>
<p>The time limit is somehow strict. Please do not spoil the problem with a cheating solution.</p>
<p>Description updated on 2010-7-11</p>