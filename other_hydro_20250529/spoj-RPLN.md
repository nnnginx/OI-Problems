<p>Orianna is a great swimmer and she's going to a swimming competition this month and needs your help as she is highly paranoic about the results of the competition.</p>
<p>The competition consists in some sort of evaluations, every judge makes a score and, based on that score and the score of other contestants she will get a score belonging to her results, those scores are final, meaning that will not change in the competition.</p>
<p> Orianna requires this solution with urgency, she is getting evaluated on a lot of ways and she is very worried about her results, so she wants to know what is the worst score from an evaluation A to other evaluation B inclusive.</p>

<h3>Input</h3>
<p>The first line of the test data will start with an integer T representing the T test cases, then, T cases will follow, each of the cases starts with two integers N and Q, denoting the number of evaluations Orianna had, then, N integers will follow denoting the score on each evaluation, after that, Q queries will begin, each query consist on two integers A and B.</p>

<h3>Output</h3>
<p>You must output the string ¡°<tt>Scenario #i:</tt>¡°, a blank line and then the result of each query, remember, Orianna is interested on the worst score from evaluation A to evaluation B inclusive.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
5 3
1 2 3 4 5
1 5
1 3
2 4
5 3
1 -2 -4 3 -5
1 5
1 3
2 4

<b>Output:</b>
Scenario #1:
1
1
2
Scenario #2:
-5
-4
-4</pre>

<h3>Constraints</h3>
<ul>
  <li>1 &lt;= T &lt;= 100</li>
</ul>
<p><b>Small input (30%):</b></p>
<ul>
  <li> 1 &lt;= N &lt;= 1,000</li>
  <li> 1 &lt;= Q &lt;= 1,000</li>
  <li> -10^9 &lt;= Ni &lt;= 10^9</li>
  <li> 1 &lt;= A &lt;= B &lt;= N</li>
</ul>
<p><b>Large input (70%):</b></p>
<ul>
  <li>1 &lt;= N &lt;= 100,000</li>
  <li>1 &lt;= Q &lt;= 100,000</li>
  <li>-10^9 &lt;= Ni &lt;= 10^9</li>
  <li>1 &lt;= A &lt;= B &lt;= N</li>
</ul>
<p><strong>Solutions rejudged due to weak test cases.</strong></p>