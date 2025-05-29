<p>New semester is coming.&nbsp; As the class monitor, <a href="../../../users/cathyyin/">Cathy Yin</a> is going to make necessary preparations.&nbsp; She has <em>m</em> jobs to do, <em>n</em> classmates are going to help her.&nbsp; Each job requires some classmates working on it for certain time, say the <em>i</em>-th classmate must work on the <em>j</em>-th job for <em>A<sub>ij</sub></em> minutes.&nbsp; As an OIer of great responsibility she wishes to finish all jobs as soon as possible.&nbsp; But a classmate can do only one job at a time, and two classmates can <strong>not</strong> do the same job at the same moment.&nbsp; For example, to decorate the classroom, Alpha must work on it for 3 minutes <strong>plus</strong> Beta works on it for 4 minutes, then one possible assignment will be ABABBAB, taking 7 minutes in total.</p>
<p>Now she is going to make a detailed schedule specifying who is doing what at each moment.&nbsp; Jobs are independent and may be done in any order.&nbsp; Also for each job anyone can do it for arbitrarily long, but <strong>not</strong> longer than the required time <em>A<sub>ij</sub></em>.&nbsp; Anyone can be free at any time.&nbsp; Time for certain classmate doing certain work need <strong>not</strong> be consecutive.</p>
<p>As her friend, you are to help her to work out the schedule minimizing the total time needed.</p>
<h3>Input</h3>
<p>First line of the input contains two positive integers <em>m</em>, <em>n</em> (1 &lt;= <em>m</em>, <em>n</em> &lt;= 2000), number of jobs and classmates.</p>
<p><em>m</em> lines follow, each descibing a job.&nbsp; <em>i</em>-th line contains <em>n</em> non-nagative integers (&lt;= 10<sup>6</sup>), where the <em>j</em>-th number is A<sub>ij</sub>, meaning that the <em>j</em>-th classmate has to work on the <em>i</em>-th job for A<sub>ij</sub> minutes as descibed above.</p>
<h3>Output</h3>
<p>First line contains single integer T, minimum time needed.&nbsp; Next line contains <em>n</em> non-negative intergers (&lt;= <em>m</em>), giving one possible schedule for the <strong>first</strong> minute, where the <em>i</em>-th number specifying the job for the <em>i</em>-th classmate to do, and 0 denotes that the corresponding classmate is free.</p>
<p>If there are multiple solutions, any one is accepted.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 2<br>2 5<br>5 1<br><br><strong>Output:</strong><br>7<br>1 0</pre>
<h4>Explanation:</h4>
<p>Two jobs are assigned to two classmates, say Lambda and Mu.&nbsp; To clean up the classroom Lambda needs to work for 2 minutes and Mu 5 minutes; and to move desks for new comers Lambda 5 minutes and Mu 1 minute.<br><br>One optimal schedule is:</p>
<table style="width: 200px;" border="0">
<tbody>
<tr>
<td>T</td>
<td>Lambda</td>
<td>Mu</td>
</tr>
<tr>
<td>0</td>
<td>Tidy</td>
<td>Free</td>
</tr>
<tr>
<td>1</td>
<td>Move</td>
<td>Tidy</td>
</tr>
<tr>
<td>2</td>
<td>T</td>
<td>M</td>
</tr>
<tr>
<td>3</td>
<td>M</td>
<td>T</td>
</tr>
<tr>
<td>4</td>
<td>M</td>
<td>T</td>
</tr>
<tr>
<td>5</td>
<td>M</td>
<td>T</td>
</tr>
<tr>
<td>6</td>
<td>M</td>
<td>T</td>
</tr>
</tbody>
</table>
<p>7 minutes in total.&nbsp; It is obvious that it is impossible to finish it in less than 7 minutes.</p>