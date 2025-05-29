<p>
You¡¯re in charge of designing a campus network between buildings and are very worried about its
reliability and its cost. So, you¡¯ve decided to build some redundancy into your network while keeping it
as inexpensive as possible. Specifically, you want to build the cheapest network so that if any one line
is broken, all buildings can still communicate. We¡¯ll call this a <i>minimal reliable net</i>.

</p><h3>Input</h3>
<p>
There will be multiple test cases for this problem. Each test case will start with a pair of integers n (&lt;=15) and m (&lt;= 20) on a line indicating the number of buildings (numbered 1 through n) and the
number of potential inter-building connections, respectively. (Values of n = m = 0 indicate the end of
the problem.) The following m lines are of the form b<sub>1</sub> b<sub>2</sub> c (all positive integers) indicating that it costs
c to connect building b<sub>1</sub> and b<sub>2</sub>. All connections are bidirectional.

</p><h3>Output</h3>
<p>
For each test case you should print one line giving the cost of a minimal reliable net. If there is a
minimal reliable net, the output line should be of the form:

</p><p></p><p>
<b><i>The minimal cost for test case p is c.</i></b>

</p><p></p><p>
where <i>p</i> is the number of the test case (starting at 1) and <i>c</i> is the cost. If there is no reliable net possible,
output a line of the form:

</p><p></p><p>
There is no reliable net possible for test case p.

</p><h3>Example</h3>

<pre><b>Input:</b>
4 5
1 2 1
1 3 2
2 4 2
3 4 1
2 3 1
2 1
1 2 5
0 0

<b>Output:</b>
The minimal cost for test case 1 is 6.
There is no reliable net possible for test case 2.
</pre>