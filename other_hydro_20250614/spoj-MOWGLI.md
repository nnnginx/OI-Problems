<p>Mowgli is a little boy brought up by a wolf pack in the jungle. The king of jungle Shere Khan wants the boy for revenge. Foreseeing his danger Akela the leader of wolf pack suggests Mowgli to leave the jungle. Before Mowgli's departure from jungle, he got the news that Shere Khan killed Akela. So Mowgli wants revenge. He wants to get back to Shere Khan's palace in shortest path.</p>
<p>There are <strong>N</strong> number of rivers in his path. Width of each river is atmost <strong>10</strong><sup><strong>5</strong> </sup>meters.&nbsp;To cross the river stones are kept at a distance of <strong>1</strong> meter. Mowgli can jump across atmost <strong>K </strong>stones at a time. Given total number of stones <strong>A<sub>i</sub></strong> kept on the <strong>i<sup>th&nbsp;</sup></strong>river. Your job is to tell total number of ways Mowgli can cross each river. As answer can be very large Give output <strong>modulo 1000000007</strong><span style="font-size: small; color: #333333; font-family: 'Open Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif; line-height: 1.1; text-align: justify;"><strong>.&nbsp;</strong></span></p>
<p style="text-align: justify; ">&nbsp;</p>
<h3>Input</h3>
<p>There are around 10 test cases.</p>
<p>First line contains an integer <strong>T</strong>&nbsp;number of test cases</p>
<p>Each test case consists of two lines:</p>
<p>First line contains two integers <strong>&nbsp;N</strong><strong>(Number of rivers)&nbsp;</strong>and&nbsp;<strong>K</strong><strong>(Maximum number of stones Mowgli can skip)</strong><strong>.</strong></p>
<p>Next line contains <strong>N</strong>&nbsp;integers. <strong>A<sub>i</sub>&nbsp;</strong><strong>(Number of stone kept on i<sup>th </sup>river).</strong></p>
<h3>Output</h3>
<p>One line for each river.</p>
<p>Total number of ways Mowgli can cross the river.</p>
<p><strong>Constraints:</strong></p>
<p>T &lt;= 10</p>
<p>1 &lt;= N &lt;= 100</p>
<p>0 &lt;= K &lt;= 50</p>
<p>0 &lt;= A<sub>i</sub>&nbsp;&lt;= 100000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>2 1</pre>
<pre>1 2

<strong>Output:</strong></pre>
<pre>2
3</pre>
<pre><strong>Explanation:</strong></pre>
<pre>For second river with 2 stones. Mowgli can jump across 1 stone maximum at a time. So there are three choices</pre>
<pre>1.<span style="white-space: pre;">	</span>Start --&gt; 1st --&gt; 2nd --&gt; Destination</pre>
<pre>2.<span style="white-space: pre;">	</span>Start --&gt; 1st --&gt; Destination</pre>
<pre>3.<span style="white-space: pre;">	</span>Start --&gt; 2nd --&gt; Destination</pre>