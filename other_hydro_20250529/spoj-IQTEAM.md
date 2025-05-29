<p>In Byteland we can study only math and IT.</p>
<p>In the university there are n math students and m IT students.</p>
<p>Rector Byteasar knows IQ of every student. He wants to make the best team, which would solve the hardest human being problems. So he decided to pick team with the highest sumarry IQ.</p>
<p>Of course it's not everything. He wants to make team in which each student knows another students from team.</p>
<p>Every student from IT know other student from IT and same with math students.</p>
<p>Help him finding team with the largest summary IQ and in which every student from team knows another students from team.</p>
<h3>Input</h3>
<p>In first line n,m,k ( 0&lt;n&lt;=400, 0&lt;m&lt;=400, 0&lt;=k&lt;=n*m ) which means number of math students, number of IT students, number of friendships between IT and math student.</p>
<p>In next k lines pairs</p>
<p>0&lt;ai&lt;=n 0&lt;bi&lt;=m, which means ai student from math knows bi student from IT.</p>
<p>In next line n numbers, IQ of i-th math student.</p>
<p>In next line m numbers, IQ of i-th IT student.</p>
<h3>Output</h3>
<p>Output in one line : number of team's summary IQ.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>3 2 3
1 1
2 1
2 2
1 3 1
1 2</pre>
<strong>Output:</strong>
<pre>6</pre>
</pre>