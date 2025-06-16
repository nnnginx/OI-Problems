<p>Friends<br><br>A group of N people are going to the movies, some pair of them are friends and according to the famous saying that "The friends of my friends are my friends, too" it follows that if A and B are friends and B and C are friends then A and C are friends, and do not forget that every friendship is mutual, if A is friend of B, then B is also friend of A.<br>They will all sit in the first row at the cinema, there are N seats in each row, a way is good if there is at least one pair of of people that are friends and at the same time they are sitting in adjacent seats. So that is your task, to count how many assignments of those N people in the N seats are good.</p>
<h3>Input</h3>
<p>Input starts with an integer T (1 &lt;= T &lt;= 600), denoting the number of test cases. Each test case starts with a line containing two integers N (2 &lt;= N &lt;= 40) and M (0 &lt;= M &lt;= 800). Each of the next M lines will contain 2 integers A B (1 &lt;= A,B &lt;= N, A != B) meaning that A and B are friends.</p>
<h3>Output</h3>
<p>For each test case print a single line with "Case #X: P" where X is the number of the test case (starting from 1) and P is the number of ways modulo 1000000007. Look at the sample output for more details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<br>3<br>2 1<br>2 1<br>3 2<br>2 1<br>1 3<br>4 0

<strong>Output:</strong><br><br>Case #1: 2<br>Case #2: 6<br>Case #3: 0
</pre>