<p>You're given a sequence <strong>s</strong> of <strong>N</strong> distinct integers.<br>Consider all the possible sums of three integers from the sequence at three different indicies.<br>For each obtainable sum output the number of different triples of indicies that generate it.<br><strong><br>Constraints:</strong><br>N &lt;= 40000, |s<sub>i</sub>| &lt;= 20000</p>
<h3>Input</h3>
<p>The first line of input contains a single integer N.<br>Each of the next N lines contain an element of s.</p>
<h3>Output</h3>
<p>Print the solution for each possible sum in the following format:<br>sum_value : number_of_triples<br><br>Smaller sum values should be printed first.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><br>5<br>-1<br>2<br>3<br>0<br>5<br><strong>Output:</strong>
<br>1 : 1<br>2 : 1<br>4 : 2<br>5 : 1<br>6 : 1<br>7 : 2<br>8 : 1<br>10 : 1<strong><br></strong></pre>
<p><strong>Explanation:</strong><br>4 can be obtained using triples ( 0, 1, 2 ) and ( 0, 3, 4 ).<br>7 can be obtained using triples ( 0, 2, 4 ) and ( 1, 3, 4 ).<br><br><strong>Note:</strong> a triple is considered the same as any of its permutations.</p>