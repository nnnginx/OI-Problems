<p>You are given a bunch of data (all are positive 32 bit numbers) to operate on. The only operations on the data are search, insert, and delete. When storing the data you have to remember its rank, that is the original position when the data is being inserted. All successful operations must return the ranks of the data. Failed operations should return NONE as the answer.</p>
<p>Your objective is to execute all of the operations as fast as possible.</p>
<h3>Input</h3>
<p>The first line of input is N and M, separated by a space, N is the  number of initial data. ( 0 &lt;= N &lt; 1000000 ) and M is the number of  operations against the data. ( 0 &lt;= M &lt; 1000000).</p>
<p>The second line contains N data, seperated by blanks. All data are positive 32 bits numbers</p>
<p>The next M lines contains operations against the data. Each line contains a symbol and a number, separated by a space.&nbsp;</p>
<p>There are 3 symbols (<strong>S</strong>, <strong>I</strong>, <strong>D</strong>), each representing search, insert, and delete operation.</p>
<p>'S  number' tries to find the number in the stored data, and outputs its  first rank in the stored data (as originally inserted), or NONE if no  such number exists.</p>
<p>'I number' inserts the number into the stored data, and outputs its rank in the stored data. (Data can be duplicated).</p>
<p>'D  number' deletes the least ranked number found in the stored data, and outpus its  rank, or NONE if no such number  originally exists.</p>
<h3>Output</h3>
<p>There is an output for each executed operation. See the above input  description about each operation for the detail of the output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>10 6<br>20 12 10 28 20 50 49 8 51 1<br>S 20<br>I 3<br>S 11<br>D 20<br>I 2<br>S 20<br><br><strong>Output:</strong><br>1<br>11<br>NONE<br>1<br>12<br>5</pre>