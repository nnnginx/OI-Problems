<p>Now a days, Ohani has become very expert in mathematics. Her teachers like her very much because of her excellent performance.&nbsp;</p>
<p>One day, one of her teacher gave her a problem to solve. He will give Ohani a number N. This will represent a table of N rows. The first row contains number from 1 to N. Then the next line will contain N-1 numbers, In the second row, the first number will be the summation of the first two numbers (1 + 2) of the previous row, the second number will be the summation of the second two numbers (2 + 3) of the previous row and so on. Row 3 will have N-2 numbers with same procedures. Same procedure follows for row 4, row 5, .... , row N. On the last row, there will be only a single number. Ohani has to tell that only number of the Nth row.</p>
<p>For example: If N = 4, then the table is:</p>
<p>1 &nbsp; 2 &nbsp; 3 &nbsp; 4</p>
<p>&nbsp;3 &nbsp; &nbsp;5 &nbsp; &nbsp;7</p>
<p>&nbsp; &nbsp; 8 &nbsp; 12</p>
<p>&nbsp; &nbsp; &nbsp;20</p>
<p>So Ohani has to answer the last remaining number: 20.</p>
<p>She can answer when N is small, but can't when N is large. Can you help her?</p>

<h3>Input</h3>
<p>The first line contains the number of testcases T (T &lt;= 100000).</p>
<p>Each of the test cases contain a number N where 1 &lt;= N &lt;= 100000.</p>

<h3>Output</h3>
<p>You have to output the case number and the required answer. As the number can be very large, output the answer modulo 1000000007.</p>
<h3>Example</h3>

<pre><strong>Input:</strong>
2<br>1<br>2

<strong>Output:</strong>
Case 1: 1<br>Case 2: 3</pre>