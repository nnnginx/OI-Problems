<h3>Problem description</h3>

<p>
Farmer John has N barren pastures (2 &lt;= N &lt;= 100,000) connected by N-1 bidirectional roads, such that there is exactly one path between any two pastures. &nbsp;Bessie, a cow who loves her grazing time, often complains about how there is no grass on the roads between pastures. &nbsp;Farmer John loves Bessie very much, and today he is finally going to plant grass on the&nbsp;roads. &nbsp;He will do so using a procedure consisting of M steps (1 &lt;= M &lt;=&nbsp;100,000).
</p>

<p>At each step one of two things will happen:</p>
<ul>
  <li>FJ will choose two pastures, and plant a patch of grass along each road in&nbsp;between the two pastures, or,</li>
  <li>Bessie will ask about how many patches of grass on a particular road, and Farmer John must answer her question.</li>
</ul>
<p>Farmer John is a very poor counter -- help him answer Bessie's questions!</p>

<h3>Input</h3>
<p>* Line 1: Two space-separated integers N and M</p>
<p>* Lines 2..N: Two space-separated integers describing the endpoints of&nbsp;a road.</p>
<p>* Lines N+1..N+M: Line i+1 describes step i. The first character of&nbsp;the line is either P or Q, which describes whether or not FJ&nbsp;is planting grass or simply querying. This is followed by two&nbsp;space-separated integers A_i and B_i (1 &lt;= A_i, B_i &lt;= N)&nbsp;which describe FJ's action or query.</p>

<h3>Output</h3>
<p>* Lines 1..???: Each line has the answer to a query, appearing in the&nbsp;same order as the queries appear in the input.</p>

<h3>Example</h3>
<h4>SAMPLE INPUT</h4>
<pre>4 6
1 4
2 4
3 4
P 2 3
P 1 3
Q 3 4
P 1 4
Q 2 4
Q 1 4</pre>

<h4>SAMPLE OUTPUT</h4>
<pre>2
1
2</pre>

<p><b>[ Edited by EB ]</b></p>
<p><b>Warning:</b> Some input files are broken.</p>