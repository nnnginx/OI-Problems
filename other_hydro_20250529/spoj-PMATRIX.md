<p style="text-align: justify;">Consider the following exercise, found in a generic linear algebra textbook.Let A be an n × n matrix. Prove that the following statements are equivalent:</p>
<ul>
<li>(a) A is invertible.</li>
<li>(b) Ax = b has exactly one solution for every n × 1 matrix b.</li>
<li>(c) Ax = b is consistent for every n × 1 matrix b.</li>
<li>(d) Ax = 0 has only the trivial solution x = 0.</li>
</ul>
<p style="text-align: justify;">The typical way to solve such an exercise is to show a series of implications. For instance,one can proceed by showing that (a) implies (b), that (b) implies (c), that (c) implies (d),and ﬁnally that (d) implies (a). These four implications show that the four statements are equivalent. Another way would be to show that (a) is equivalent to (b) (by proving that (a) implies (b) and that (b) implies (a)), that (b) is equivalent to (c), and that (c) is equivalent to (d).</p>
<p style="text-align: justify;"><br>However, this way requires proving six implications, which is clearly a lot more work than just proving four implications! I have been given some similar tasks, and have already started proving some implications. Now I wonder, how many more implications do I have to prove? Can you help me determine this ?</p>
<h3>Input</h3>
<p>On the ﬁrst line one positive number: the number of testcases, at most 100. After that per testcase:</p>
<ul>
<li style="text-align: justify;"> One line containing two integers n (1 ≤ n ≤ 20 000) and m (0 ≤ m ≤ 50 000): the number of statements and the number of implications that have already been proved.</li>
<li style="text-align: justify;">m lines with two integers s1 and s2 (1 ≤ s1, s2 ≤ n and s1 = s2) each, indicating that it has been proved that statement s1 implies statement s2.</li>
</ul>
<h3>Output</h3>
<p style="text-align: justify;">Per testcase:<br>One line with the minimum number of additional implications that need to be proved in order to prove that all statements are equivalent.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>4 0<br>3 2<br>1 2<br>1 3<br><br><strong>Output:</strong><br>4<br>2<br></pre>