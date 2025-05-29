<p>You have an array of problems <strong>A</strong> with <strong>N</strong> problems. Each problem has a Difficulty level. <strong>i-th </strong>has dificulty <strong>A[i]</strong>. <br><br>You want to give this problems to HrSiam. But you know, HrSiam doesn't like easy problems, so he will get angry. Also he doesn't want to solve problems with same difficulty again and again. <br><br>So he also has an array Angry, with N elements.</p>
<p>When he visits a problem with certain difficulty <strong>d</strong>, his angriness will increase by <strong>d * angry[1]</strong>.<br>After some time if he again visits a problem with same difficulty, for the second time, then his angriness will increase by <strong>d * angry[2]</strong>, and so on.<br>Basically, if he visit a problem with certain difficulty <strong>d </strong>for the <strong>i-th </strong>time, his angrines will increase by <strong>d * angry[i]. </strong></p>
<p>In this circumstances, you want to do 2 things - <br>1. You are afrad that HrSiam may get too angry, so you want to present a part of the array to him. But you need to quickly determine what will be his total angriness if you present the sub array of problems <strong>A[l...r]</strong> to HrSiam? <br>2. After certain time you may want to change difficulty of a problem, i.e set difficulty of <strong>x-th</strong> problem to<strong> y</strong>.</p>
<h3>Input</h3>
<p>First line there will an integer <strong>N</strong>, the number of problems you have.</p>
<p>Next line will contain the difficulty of the problems, the array <strong>A[].&nbsp; </strong></p>
<p>Next line will contain the array <strong>angry[], </strong>of length <strong>N</strong>.</p>
<p>Next line, there will be an integer <strong>Q</strong>, the number of queries you want to make.</p>
<p>Next <strong>Q</strong> lines will describe the queries, in format -</p>
<p><strong>t x y </strong></p>
<p>If t is one, then you need to find the total angriness of the Subarray <strong>A[l...r]</strong> when presented to HrSiam. <br>Else you need to set<strong> A[x] = y</strong>.</p>
<h3>Constrains</h3>
<p><strong>1 &lt;= N, Q, x, y, A[i], angry[i] &lt;= 100000&nbsp;</strong></p>
<p><strong>If x, y is in query of first type, then 1 &lt;= x &lt;= y &lt;= N &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong></p>
<h3>Output</h3>
<p>For each query of first type, print an integer, the total angriness of the subarray. Solutions to the queries should be printed in the order they appeared in the input.</p>
<h3>Explanation of Sample</h3>
<p>In the first sample, the first query range is <strong>[3, 6]</strong>, the array elements are <strong>{3, 3, 1, 1}</strong>. <br>When HrSiam see the first problem with difficulty 3, his angriness will increase by <strong>3 * angry[1]</strong>. <br>Then he visit a problem with same difficulty he saw before, for the second time, so add <strong>3 * angry[2] </strong><br>Then<strong> 1 * angry[1]</strong> and <strong>1 * angry[2] <br>Total = (3 * 1) + (3 * 2) + (1 * 1) + (1 * 2) = 12</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8<br>1 2 3 3 1 1 2 3 <br>1 2 3 4 5 6 7 8<br>2<br>1 3 6 <br>1 1 5 <br><br><strong>Output:</strong>
12<br>14 <br></pre>