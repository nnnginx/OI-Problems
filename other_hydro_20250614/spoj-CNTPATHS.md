<p>John likes to take a walk from his house to university. He needs to arrive his university in at most <strong>T</strong> seconds after leaving his home. We can represent the situation as a <strong>N</strong> vertices graph. Vertex 0 of the graph will be John's home and vertex 1 John's university. There can be bidirectional roads connecting pairs of vertices, each road will take John some seconds to cross.</p>
<p>John likes variety. We consider a valid path to be a sequence of vertices that starts with vertex 0 (John's house) and finishes with vertex 1 (The University) and there exists a road connecting each pair of consecutive vertices in the sequences (Note that a vertex may appear multiple times in the path). The total time John needs to traverse a path is equal to the sum of the times needed to cross each individual road in it. Please count the total number of different paths that need at most <strong>T</strong> minutes to be traversed in total. Two paths are different if there is at least one moment at which they visit different vertices.</p>
<p>Given <strong>T</strong>, <strong>N</strong> and the roads between the vertices,&nbsp; ¿How many different paths that need at most <strong>T</strong> seconds exist? Print the result modulo 1000000007&nbsp; (10<sup>9</sup>+7).</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line consists of a integer <strong>TOTAL</strong>, the total number of test cases (1 &lt;= <strong>N</strong> &lt;= 10).</p>
<p>Each of the following test cases begins with a single line that contains two integers : <strong>N</strong> and <strong>T</strong>. (2 &lt;= <strong>N</strong> &lt;= 5), (1 &lt;= <strong>T</strong> &lt;= 1000000000 (10<sup>9</sup>) ).</p>
<p>The <strong>N</strong> following lines are indexed from <strong>i</strong>=0 to <strong>N</strong>-1. &nbsp; The <strong>i-th</strong> line will represent the roads that connect vertex <strong>i</strong>&nbsp; with other vertices. The line will consist of <strong>N</strong> character&nbsp; indexed from <strong>j=</strong>0 to <strong>N</strong>-1<strong>.&nbsp;</strong> The <strong>j</strong>-th character of the <strong>i</strong>-th line represents the road connecting vertex <strong>i</strong> with vertex <strong>j</strong>. If the character is '-', this means no road connectes vertices <strong>i</strong> and <strong>j</strong>. Otherwise, the character will be a digit equal to 1,2 or 3, determining the number of minutes it takes John to move between vertices <strong>i</strong> and <strong>j</strong>.</p>
<p>For every pair (<strong>i</strong>,<strong>j</strong>), the road character between <strong>i</strong> and <strong>j</strong> will be the same as the one between <strong>j</strong> and <strong>i</strong>.</p>
<p>For each <strong>i</strong>, there will never be a road cannecting vertex <strong>i</strong> with itself.</p>
<p>Vertex 0 represents John's house and Vertex 1 John's university.</p>
<h3>Output</h3>
<p>For each test case, show in a single line: "Case #i: R", where R is the total number of valid paths between vertices 0 and 1 donde R that need a quantity of at most <strong>T</strong> segundos .</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>2 9<br>-3<br>3-<br>5 4<br>--123<br>--123<br>11---<br>22---<br>33---<br>3 100<br>-21<br>2-3<br>13-

<strong>Output:</strong>
Case #1: 2<br>Case #2: 4<br>Case #3: 924247768
</pre>
<h3>Notes</h3>
<p>There are two paths in the first case that need 9 minutes or less:</p>
<ul>
<li>0 -&gt; 1 (3 minutes)</li>
<li>0 -&gt; 1 -&gt; 0 -&gt; 1 (9 minutes)</li>
</ul>
<p>The second case contains 4 paths that need at most 4&nbsp; minutes to be traversed:</p>
<ul>
<li>0 -&gt; 2 -&gt; 1 (2 minutes)</li>
<li>0 -&gt; 3 -&gt; 1 (4minutes)</li>
<li>0 -&gt; 2 -&gt; 0 -&gt; 2 -&gt; 1 (4 minutes)</li>
<li>0 -&gt; 2 -&gt; 1 -&gt; 2 -&gt; 1 (4minutes)</li>
</ul>
<p>0 -&gt; 4 -&gt; 1 is a path that needs 6 minutes.</p>
<p>&nbsp;</p>