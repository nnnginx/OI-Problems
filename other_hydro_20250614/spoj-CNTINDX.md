<p>Let's deal with an array, the most important data structure of computer science. You will be given some operations to do. There will be three types of operations:</p>
<p>Type 1: Insert a number at the end of the array.</p>
<p>Type 2: Delete the last number of the array, where the last number means the latest number which has been inserted.</p>
<p>Type 3: You will get a number and two indices i &amp; j where i&lt;=j. Now you will have to answer how many time the number appears in the array starting from i to j.</p>
<p>You may assume that initially the array is empty.</p>
<h3>Input</h3>
<p>Each file contains one test case. The first line is an integer Q(1&lt;=Q&lt;=200000), the number of operations. Each of the next Q lines contains an opeation. The operations will appear as the formats below:</p>
<p>1 x , where 1&lt;=x&lt;=200000, which means you have to insert number x at the end of the array.</p>
<p>0 , For this operation, you have to delete the last number of the array</p>
<p>2 x i j , Here, you have to find how many times x appers in the array from i to j. Here x will always be present in the array and 1&lt;=i&lt;=j&lt;=length the array.</p>
<h3>Output</h3>
<p>For deletion, if the array is already empty, then output a string "invalid" (without quote),otherwise you don't need to print anything for deleting numbers. For the operation type of 2, you have to output an integer, how many times x appears in the array from i to j inclusive.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>7<br>1 10<br>1 20<br>2 20 1 2<br>0<br>2 10 1 1<br>0<br>0&nbsp;</pre>
<pre><strong>Output:</strong>
1<br>1<br>invalid&nbsp;</pre>