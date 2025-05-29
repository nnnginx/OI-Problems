<p>There are N people and M teams. Each team is a subset of N people.</p>
<p>For each team, we need to pick a captain. <b>No people could be a captain of more than one team.</b></p>
<p>A person <b>a</b> is said to be a subordinate of a person <b>b</b> if there is some team including both a and b in which b is the captain.</p>
<p>A captain selection process is said to be valid if we could not find a sequence of more than 2 people a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>k</sub> such that ai is a subordinate of a<sub>i+1</sub> (i &lt; k) and a<sub>k</sub> is a subordinate of a<sub>1</sub>.</p>
<p>For example, if we have 4 people and 3 teams:</p>
<pre>Team 1: {1, 2, 3}
Team 2: {2, 3, 4}
Team 3: {3, 4, 1}
</pre>
<p>The captain selection process:</p>
<pre>Captain 1: 1
Captain 2: 2
Captain 3: 4
</pre>
<p>is not valid since 1 is a subordinate of 4, 4 is a subordinate of 2 and 2 is a subordinate of 1.</p>

<p>Your job is to determine a valid captain selection process.</p>

<h3>Input</h3>
<p>The first line contains a number t (about 10), which is the number of test cases. Then t test cases
follow. Each test case has the following form.</p>
<p>The first line contains two numbers N and M (1 ¡Ü N, M ¡Ü 50). </p>
<p>
Each of the M teams is described in the next 2 lines. 
The first line contains the number of people in the team. <b>Each team has either 2 or 3 people.</b>
The second line contains the indexes (1-based) of the people in that team.
</p>
<p>
There is a blank line after each test case's input.
</p>

<h3>Output</h3>
<p>
For each test case, print a number -1 if there is no valid captain selection process.
</p>
<p>
Otherwise, print M lines, each line contains the index of the captain of the corresponding team.
</p>
<p>
Print a blank line after each test case's output.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4 3
3
1 2 3
3
2 3 4
3
3 4 1

4 3
3
1 2 3
2
2 4
3
3 4 2

<b>Output:</b>
-1

1
2
3
</pre>