<p>You may perhaps know how to find the last nonzero digit of n factorial. This time your task is harder, find the last nonzero decimal digit of the multinomial coefficient:<br> (a<sub>1</sub>+a<sub>2</sub>+ ¡­ +a<sub>n</sub>)!/(a<sub>1</sub>!*a<sub>2</sub>!* ¡­ *a<sub>n</sub>!) . Note that this is an extension of the classical problem, since factorials (and binomial numbers) are also multinomial numbers!</p>
<h3>Input</h3>
<p>An integer <em>T</em>, denoting the number of testcases (<em>T</em>¡Ü10000). In each line you are given one positive integer ( n¡Ü20 ), followed by n integers: a<sub>1</sub>,a<sub>2</sub>,¡­,a<sub>n</sub>, where 0 ¡Ü a<sub>i</sub> ¡Ü 1000000000. There are 4 input sets for 10 points.</p>
<h3>Output</h3>
<p>Output <em>T</em> lines, the case number followed by the last nonzero decimal digit. See the sample output for the correct format!</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7
1 0
2 11 9
4 5 7 2 9
3 1000 3000 2000
3 100000000 200000000 300000000
2 4 9
8 1 1 4 7 4 8 9 2

<strong>Output:</strong>
Case 1: 1
Case 2: 6
Case 3: 8
Case 4: 6
Case 5: 2
Case 6: 5
Case 7: 4
</pre>
<h3>Warning: A naive algorithm will probably solve only the first two input sets (4 pts).</h3>