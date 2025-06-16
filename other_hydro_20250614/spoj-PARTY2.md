<p><em>N</em> (1&lt;= <em>N</em> &lt;=100000) perfect killers (we number them 1, 2, 3, ..., <em>N</em>) meet at Blue Mary's house. Every killer has a kind of skill - cloak. No one can see them when they are cloaked - except only a small group of people, which will be discussed later.</p>
<p>We can group these killers into <em>M</em> (<em>M</em> &gt;=3) groups, called group No.1, group No.2, group No.3, etc. If killer A is in group No. <em>x</em> and killer B is in group No. (<em>X</em>%<em>M</em>+1), A can see B even if B is cloaked. This prevent killers from doing some bad things without the risk of being punished.</p>
<p>To keep their identity secret, every killer keep cloaked during the party. After the party, Blue Mary asked everyone a question, "Which killers can you see in the party?" Although some killers forget some person they have ever seen during the party, Blue Mary collects extremely much information. Now she needs you help to determine the value of <em>M</em>, because no killer is willing to share this value with her.</p>
<h3>Input</h3>
<p>Ten test cases(given one after another, you have to process all!). For each test case:</p>
<p>The first line contains two integers <em>N</em> and <em>E</em>(1&lt;= <em>E</em>&lt;= 180000). E lines follow, each line contains two space-seperated integers A and B - killer No. A can see killer No.B even if he is cloaked.</p>
<h3>Output</h3>
<p>For each test case, output one line:</p>
<p>If the information given is contradictory, output one line "-1 -1". Otherwise output the largest and the smallest possible value of <em>M</em>, seperated by a single space.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 5
1 2
2 3
3 4
4 1
3 5
3 3
1 2
2 1
2 3
[and 8 test cases more]

<strong>Output:</strong>
4 4
-1 -1
[and 8 test cases more]</pre>
<p><strong>Warning: large input/output data, be careful with certain languages</strong></p>