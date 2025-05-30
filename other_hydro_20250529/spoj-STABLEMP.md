<p>There are given <i>n</i> men and <i>n</i> women. Each woman ranks all men in order of her preference (her first choice, her second choice, and so on). Similarly, each man sorts all women according to his preference. The goal is to arrange <i>n</i> marriages in such a way that if a man <i>m</i> prefers some woman <i>w</i> more than his wife, then <i>w</i> likes her husband more than <i>m</i>. In this way, no one leaves his partner to marry
somebody else. This problem always has a solution and your task is to find one.

</p><h3>Input</h3>
<p>The first line contains a positive integer <i>t</i> &lt;= 100 indicating the number of test cases. Each test case is an instance of the stable marriage problem defined above.
The first line of each test case is a positive integer <i>n</i> &lt;= 500 (the number of marriages to find).
The next <i>n</i> lines are the <b>woman</b>'s preferences: <i>i</i>th line contains the number <i>i</i> (which means that this is the list given by the <i>i</i>th woman) and the numbers of men (the first choice of <i>i</i>th woman, the second choice,...). Then, the <b>men</b>'s preferences follow in the same format.

</p><h3>Output</h3>
<p>For each test case print <i>n</i> lines, where each line contains two numbers <i>m</i> and <i>w</i>, which means that the <b>man</b> number <i>m</i> and the <b>woman</b> number <i>w</i> should get married.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4
1 4 3 1 2
2 2 1 3 4
3 1 3 4 2
4 4 3 1 2
1 3 2 4 1
2 2 3 1 4
3 3 1 2 4
4 3 2 4 1
7
1 3 4 2 1 6 7 5
2 6 4 2 3 5 1 7
3 6 3 5 7 2 4 1
4 1 6 3 2 4 7 5
5 1 6 5 3 4 7 2
6 1 7 3 4 5 6 2
7 5 6 2 4 3 7 1
1 4 5 3 7 2 6 1
2 5 6 4 7 3 2 1
3 1 6 5 4 3 7 2
4 3 5 6 7 2 4 1
5 1 7 6 4 3 5 2
6 6 3 7 5 2 4 1
7 1 7 4 2 6 5 3

<b>Output:</b>
1 3
2 2
3 1
4 4
1 4
2 5
3 1
4 3
5 7
6 6
7 2</pre>

<b>Warning: large Input/Output data, be careful with certain languages</b>