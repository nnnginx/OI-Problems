<p>Planning Poker, also called Scrum poker, is a consensus-based technique for estimating, mostly used to estimate effort or relative size of user stories in software development.<br>
A typical Planning Poker Deck has cards showing the Fibonacci sequence including a zero: 0, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89. other decks use similar progressions.<br>
We have some tasks estimated with other complexities from 1 to 10000000.<br>
We need to estimate the complexity of all tasks using the Fibonacci sequence used in Planning Poker. The rule is that the old complexity will change to the valid complexity more close. But if two complexities are in equal distances take the higher.<br>
</p><h3>Input</h3>
<p>The input consists of multiple test cases.<br>
Each test case begins with a line containing an integer ¡°N¡± (1 &lt;= N &lt;= 100000) the number of tasks. In the following line are the complexities of "N" tasks from "0" to "N-1" (1 &lt;= task[i] &lt;= 10000000).<br>
The end of input is indicated by a line with one zero. This is not a part of any test cases.<br>
</p><h3>Output</h3>
<p>For each test case print the list of new complexities sorted in ascending order. Print a space character between two complexities.<br>
</p><h3>Example</h3>
<pre><b>Input:</b>
5
1 2 3 4 5
5
7 8 9 11 10
0

<b>Output:</b>
1 2 3 5 5
8 8 8 8 13

</pre>