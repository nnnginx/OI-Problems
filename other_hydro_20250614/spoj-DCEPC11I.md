<p>Vaibhav Sir and Saikat Sir, after completing their graduation, got a job together at a store.</p>
<p>Their boss at the store was Sidharth Sir, who was very strict and did not want anyone to have fun at the job. He gave Vaibhav and Saikat sir a very boring job of stacking columns of boxes in a row of size N.</p>
<p>To make it a little interesting, both of them decided that whenever they need to add more boxes, they will choose st and en, such that 1&lt;=st&lt;=en&lt;=N, and place 1 box in column st, 2 boxes in column st+1, бн and (en-st+1) boxes in column en.</p>
<p>When Sidharth sir saw this, he decided to have some fun of his own, and asked them to count the number of boxes in all columns from st to en, and tell him the result. Now Vaibhav and Saikat sir have come to you for help to answer the queries of their boss, as they do not want to lose their jobs.</p>
<h3>Input</h3>
<p>The first line contains N, the number of columns and Q, the number of queries.</p>
<p>The next Q lines can be of the following form иC</p>
<p>1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 0 st en, meaning Vaibhav and Saikat sir add boxes to the columns from st to en as described above.</p>
<p>2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1 st en, meaning Sidharth sir asks them to count the number of boxes in all columns from st to en.</p>
<h3>Output</h3>
<p>For all queries of type 2, output a line containing the answer to the query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 6<br>0 2 4<br>1 1 5<br>0 1 5<br>0 3 5<br>1 1 5<br>1 3 5

<strong>Output:</strong>
6<br>27<br>23
</pre>
<pre><p><strong>Constraints:</strong></p><p>1&lt;=N, Q&lt;=100000</p></pre>