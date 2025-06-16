<p>You've been to a potluck party (party where each person contributes food), but some people are angry that they spent more money preparing their dish than the others. Now they want you (they span the bottle) to figure out how the participants of the party can, in the <em>fewest</em> amount of transfers, become even.</p>
<p>To clarify, you are free to transfer money between them in any way you like, but eventually the money they spent on their dishes, plus the money they received, minus the money the sent, must be equal for all participants.</p>
<h3>Input</h3>
<p>The first line contains C&nbsp;�� [0..10] - the number of test cases.</p>
<p>For each test case, the first line contains the number N �� [0..20] - the number of people at the party.</p>
<p>The following N lines contains a interger x<sub>i</sub>&nbsp;�� [0,10^6] representing the amount of money the ith persons dish cost.</p>
<h3>Output</h3>
<p>For each testcase:</p>
<p>The first line should be the minimal amount of transfers needed to even out the party budget.</p>
<p>The following lines should be on the form "a -&gt; b: t", where a,b �� [0..N) and represent that person 'a' must transfer 't' money to person 'b'. t is here a floating point number of at least 6 digits precision. (Notice: that is 6 digits precision after adding together your in and out flows)</p>
<p>In case of multiple best solutions exists, print any.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
<strong>6</strong>
2
4
1
5
0
6
<strong>3</strong>
9
16
25
</pre>
<pre><strong>Output:</strong>
3
0 -&gt; 1: 1.0
2 -&gt; 3: 2.0
4 -&gt; 5: 3.0
2
0 -&gt; 1: 7.6666666666667
1 -&gt; 2: 8.33333333333</pre>
<pre><strong>Explaination:</strong></pre>
<p>In the first case, 3 is the minimal amount of transfers. An alternative transfer pattern would be "0 -&gt; 3: 1 &nbsp; &nbsp;1 -&gt; 3: 2 &nbsp; &nbsp;2 -&gt; 4: 2 &nbsp; &nbsp; 2 -&gt; 5: 1". That would have made everyone even, but would have taken one more transfer (4).</p>
<p>In the second case, after the transfers, each person is down 16.666.</p>