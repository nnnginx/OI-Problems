<p>As another one of their crazy antics, the N (1 �� N �� 100,000) cows want Farmer John to race against the clock to answer some of their pressing questions.</p>

<p>The cows are lined up in a row from 1 to N, and each one is holding a sign representing a number, A<sub>i</sub> (1 �� A<sub>i</sub> �� 1,000,000,000). The cows need FJ to perform Q (1 �� Q �� 50,000) operations, which can be either of the following:</p>

<ul>
<li>Modify cow i's number to X (1 �� X �� 1,000,000,000). This will be represented in the input as a line containing the letter M followed by the space-separated numbers i and X.</li>

<li>Count how many cows in the range [P, Q] (1 �� P �� Q �� N) have A<sub>i</sub> �� X (0 �� X �� 1,000,000,000). This will be represented in the input as a line containing the letter C followed by the space-separated numbers P, Q, and X.</li>
</ul>

<p>Of course, FJ would like your help.</p>

<h3>Input</h3>
<p>The first line gives the integers N and Q, and the next N lines give the initial values of A<sub>i</sub>. Finally, the next Q lines each contain a query of the form "M i X" or "C P Q X".</p>

<h3>Output</h3>
<p>Print the answer to each 'C' query, one per line.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4 6
3
4
1
7
C 2 4 4
M 4 1
C 2 4 4
C 1 4 5
M 2 10
C 1 3 9

<b>Output:</b>
2
3
4
2
</pre>

<p>FJ has 4 cows, whose initial numbers are 3, 4, 1, and 7. The cows then give him 6 operations; the first asks him to count the how many of the last three cows have a number at most 4, the second asks him to change the fourth cow's number to 1, etc.</p>

<b>Warning: large input/output data.</b>