<h3>Background</h3>
<p><em>To The Moon</em> is a <a href="http://www.igf.com/">independent&nbsp;game</a>&nbsp;released in November 2011, it is a role-playing adventure game powered by&nbsp;<a title="RPG Maker" href="http://en.wikipedia.org/wiki/RPG_Maker">RPG Maker</a>.</p>
<p style="text-align: center;"><img title="River &amp;&amp; Anya .. ." src="./24786/file/4ADkMizY.png" alt="River &amp;&amp; Anya .. ." width="640" height="480"></p>
<p>The premise of <em>To The Moon</em> is based around a technology that allows us to permanently reconstruct the memory on dying man. In this problem, we'll give you a chance,&nbsp;to implement the logic behind the scene.</p>
<h3>Description</h3>
<p>You¡®ve been given N integers A[1], A[2],..., A[N]. On these integers,&nbsp;you need to implement the following operations:</p>
<ul>
<li>C l r d: Adding a constant d for every {Ai | l &lt;= i &lt;= r}, and increase the timestamp by 1, this is the only operation that will cause the timestamp increase.&nbsp;</li>
<li>Q l r: Querying the current sum of {Ai | l &lt;= i &lt;= r}.</li>
<li>H l r t: Querying a history sum of {Ai | l &lt;= i &lt;= r} in time t.</li>
<li>B t: Back to time t. And once you decide return to a past, you can never be access to a forward edition anymore.</li>
</ul>
<p>&nbsp;.. N, M ¡Ü 10^5, |A[i]| ¡Ü 10^9, 1 ¡Ü l ¡Ü r ¡Ü N, |d| ¡Ü 10^4 .. the system start from time 0, and the first modification is in time 1, t ¡Ý 0, and won't introduce you to a future state.&nbsp;</p>
<h3>Input</h3>
<pre>n m<br>A1 A2 ... An<br>... (here following the m operations. )</pre>
<h3>Output</h3>
<pre>... (for each query, simply print the result. )</pre>
<h3>Example</h3>
<pre><pre style="text-align: left;"><strong>Input 1:</strong><br>10 5
1 2 3 4 5 6 7 8 9 10
Q 4 4
Q 1 10
Q 2 4
C 3 6 3
Q 2 4<br><br><strong>Output 1:</strong><br>4
55
9
15<br><strong><br>Input 2:<br></strong>2 4
0 0
C 1 1 1
C 2 2 -1
Q 1 2
H 1 2 1<br><strong><br>Output 2:</strong><br>0
1</pre>
</pre>