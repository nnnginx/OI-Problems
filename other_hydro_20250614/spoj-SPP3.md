<p>Sequence <em>(a<sub>i</sub>)</em> of natural numbers is defined as follows:<br><br> <em>a<sub>i</sub> = b<sub>i</sub></em> if <em>i ¡Ü k</em><br> <em>a<sub>i</sub> = c<sub>1</sub>a<sub>i-1</sub> + c<sub>2</sub>a<sub>i-2</sub> + ... +  c<sub>k</sub>a<sub>i-k</sub></em> if <em>i &gt; k</em><br><br> where <em>b<sub>j</sub></em> and <em>c<sub>j</sub></em> are given natural numbers for <em>1 <em>¡Ü j <em>¡Ü </em></em>k</em>. Your task is to compute <em>a<sup>2</sup><sub>m</sub></em> + <em>a<sup>2</sup><sub>m+1</sub></em> + <em>a<sup>2</sup><sub>m+2</sub></em> + ... + <em>a<sup>2</sup><sub>n</sub></em> for given <em>m</em> <em>¡Ü</em> <em>n</em> and output it modulo a given positive integer <em>p</em> (not necessarily prime).</p>
<h3>Input</h3>
<p>On the first row there is the number <em>T</em> of test cases (<em>T</em> <em>¡Ü </em>50).<br> Each following test case contains four lines:</p>
<ul>
<li> <em>k</em> - number of elements of <em>(c)</em> and <em>(b)</em> (<em>1 <em>¡Ü</em> k <em>¡Ü</em> 15</em>)</li>
<li> <em>b<sub>1</sub>,...,b<sub>k</sub></em> - <em>k</em> natural numbers where <em>0 <em>¡Ü</em> b<sub>j</sub> <em>¡Ü</em> 10<sup>9</sup></em> separated by spaces</li>
<li><em>c<sub>1</sub>,...,c<sub>k</sub></em> - <em>k</em> natural numbers where <em>0 <em>¡Ü</em> c<sub>j</sub> <em>¡Ü</em> 10<sup>9</sup></em> separated by spaces</li>
<li><em>m</em>, <em>n</em>, <em>p</em> - natural numbers separated by spaces (<em>1 <em>¡Ü</em> m <em>¡Ü</em> n <em>¡Ü</em> 10<sup>18</sup></em>, <em>1 <em>¡Ü</em> p <em>¡Ü</em> 10<sup>8</sup></em>)</li>
</ul>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Exactly <em>T</em> lines, one for each test case:  (<em>a<sup>2</sup><sub>m</sub></em> + <em>a<sup>2</sup><sub>m+1</sub></em> + <em>a<sup>2</sup><sub>m+2</sub></em> + ... + <em>a<sup>2</sup><sub>n</sub></em>) modulo <em>p</em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3<br>2 3 5<br>1 2 3<br>10 15 1000000<br>15<br>401 131 940 406 673 592 532 452 733 966 602 600 61 212 257<br>13 12 81 75 37 12 10 35 25 75 16 90 27 33 47<br>2 85704376 99999991

<strong>Output:</strong>
248783<br>32397016
</pre>
<h3>Note</h3>
<p>You can try the problem <a href="../../problems/SPP/">SPP</a> first.</p>