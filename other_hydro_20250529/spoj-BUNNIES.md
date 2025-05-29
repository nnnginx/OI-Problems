<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Pompom bunny has N strange eggs. The i-th egg is broken by tapping it exactly Ai times. Pompom</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">needs to break K eggs as soon as possible for cooking a rice omelet. However she has been put in an</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">uncomfortable situation. Someone has shuffled the eggs! Pompom knows the values Ai, however she</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">doesn't know which egg is which. She'd like to minimize the worst-case number of taps. What is the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">minimal number?</div>
<p>&nbsp;</p>
<p>Pompom bunny has N strange eggs. The i-th egg is broken by tapping it exactly Ai times. Pompom</p>
<p>needs to break K eggs as soon as possible for cooking a rice omelet. However she has been put in an</p>
<p>uncomfortable situation. Someone has shuffled the eggs! Pompom knows the values Ai, however she</p>
<p>doesn't know which egg is which. She'd like to minimize the worst-case number of taps. What is the</p>
<p>minimal number?</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line contains an integer T, the number of test cases. Then T test cases follow. The first line for</p>
<p>each test case has 2 integers N and K. Then next line has N integers A1, A2, ..., AN.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case, print the minimal number of taps for the worst-case.</p>
<p>&nbsp;</p>
<p>Constraints</p>
<p>1 &lt;= T &lt;= 10</p>
<p>1 &lt;= K &lt;= N &lt;= 3000</p>
<p>1 &lt;= Ai &lt;= 1000000 (106)</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>2 1</pre>
<pre>5 8</pre>
<pre>2 1</pre>
<pre>5 58</pre>
<pre>3 2</pre>
<pre>1 2 3</pre>
<pre><strong>Output:</strong>
8</pre>
<pre>10</pre>
<pre>5</pre>
<pre>Output details
In the first case, if a egg isn't broken after 5 taps, she should continue to tap the same egg.
In the second case, if a egg isn't broken after 5 taps, she should tap another egg 5 times.
</pre>