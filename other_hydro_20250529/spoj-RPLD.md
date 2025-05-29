<p>Gaby enjoy working in a database of a very important university, this university has students of course, each student can see as many subjects they want, however, the database suffered an attack by a group of hackers, now, Gaby needs to see the backup files, but then she noticed that some of the backup files are corrupted as well... For example, the backup file can show that a student is seeing 2 same subjects, desperate, she needs help on this task.</p>

<p>It is known that several students (different ones) can see the same subject, however, one single student cannot see the same subject (this would seem ridiculous), if one student sees the same subject two or more times, this test would belong to a corrupted file.</p>

<h3>Input</h3>
<p>First line will contain an integer T, representing the cases to evaluate, the next T cases will start with a N and R, both integers, denoting the number of students and the number of lines the database have, the next R lines contains two integers I and C, I stands for the ID of the students and C for the subject code.</p>

<h3>Output</h3>
<p>You will output T lines for each test case, starting with the string ¡°<tt>Scenario #i: </tt>¡° where i is the test case you're evaluating, then, you should output the string ¡°impossible¡± if the database file on evaluation is corrupted and the string ¡°possible¡± if its not.</p>

<h3>Example</h3>
<pre><strong>INPUT:</strong>
2
2 4
1 6102
1 6103
2 6102
2 6103

2 4
1 6102
1 6102
2 6102
2 6103

<b>Output:</b>
Scenario #1: possible
Scenario #2: impossible
</pre>


<h3>Constraints</h3>
<p>
1 &lt;= N &lt;= 10000<br>
1 &lt;= R &lt;= 100000<br>
1 &lt;= I &lt;= N<br>
1000 &lt;= C &lt;= 9999
</p>