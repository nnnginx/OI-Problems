<p>Having crossed the first hurdle, Mario encounters a long and narrow alleyway, with turtles. Mario can cross it by jumping from one turtle to another. Whenever Mario makes his jump on any given turtle, he can leave it in any of the three possible states, as per his choice. These states are:</p>
<ul>
<li>Active (A)</li>
<li>Dormant (D)</li>
<li>Bruised (B)</li>
</ul>
<p>
There are n turtles in the street, indexed 0..(n-1). Each jump costs some amount of energy, which depends on the index of turtle as well as the state it is left in. However, Mario has to take care that no neighboring turtles are left in the same state, or otherwise they all will reunite and cause a fatal attack on Mario, as he is about to leave the alley.</p>
<p>
The neighbors of turtle i are turtles i-1 and i+1. (<b>Edited:</b> If n &gt;= 3,) The first and last turtles are not neighbors.
</p> 

<p>
You need to find out the minimum amount of energy required to cross the alley.
</p>

<h3>Input</h3>
<p>
first line contains no. of test cases T (T &lt;= 5) <br>
T input sets are given in the following manner:
</p><ul>
  <li>the first line contains n, no. of turtles (n &lt;= 20) </li>
  <li>the next n lines have space separated 3 numbers (a1, a2, a3), the values of energy needed for ith turtle to change into states A D B (0 &lt;= ai &lt;= 1000) </li>
  <li>similarly, the inputs are given for other cases</li>
</ul>
<p></p>

<h3>Output</h3>
<p>
T lines, the minimal energy needed for each set of input
</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
3
0 1 2
1 4 8
9 2 5
4
10 10 10
2 4 9
12 7 10
6 6 6

<b>Output:</b>
4
25</pre>