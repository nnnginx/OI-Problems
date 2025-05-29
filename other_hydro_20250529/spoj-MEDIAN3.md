<p>When Mr. B, Mr. G and Mr. M were preparing for the 2012 ACM-ICPC World Final Contest, Mr. B had collected a large set of contest problems for their daily training. When they decided to take training, Mr. B would choose one of them from the problem set. All the problems in the problem set had been sorted by their time of publish. Each time Prof. S, their coach, would tell them to choose one problem within a particular publish time interval. That is to say, if problems had been sorted in a line, each time they will choose one of them from a specified segment of the line.</p>
<p>Moreover, when collecting the problems, Mr. B had also known an estimation of the difficulty of each problem. When he was asked to choose a problem, if he chose the easiest one, Mr. G would complain that ��Hey, what a trivial problem!��; if he chose the hardest one, Mr. M would grumble that it took too much time to finish it. For addressing this dilemma, Mr. B decided to take the one with the medium difficulty. Therefore he needed a way to know the median number in the given interval of the sequence.</p>
<h3>Input</h3>
<p>For each test case, the first line contains a single integer <strong>n</strong> (1 &lt;= <strong>n</strong> &lt;= 100,000) indicating the total number of problems. The second line contains <strong>n</strong> integers <strong>x<sub>i</sub></strong> (0 &lt;= <strong>x<sub>i</sub></strong> &lt;= 1,000,000,000), separated by single space, denoting the difficulties of each problem, already sorted by publish time. The next line is a single integer <strong>m</strong> (1 &lt;= <strong>m</strong> &lt;= 100,000), specifying number of queries. Then m lines follow, each line contains a pair of integers, <strong>A</strong> and <strong>B</strong> (1 &lt;= <strong>A</strong> &lt;= <strong>B</strong> &lt;= <strong>n</strong>), denoting that Mr. B needed to choose a problem between positions <strong>A</strong> and <strong>B</strong> (inclusively, positions are counted from 1). It is guaranteed that the number of items between <strong>A</strong> and <strong>B</strong> is odd.</p>
<h3>Output</h3>
<p>For each query, output a single line containing an integer which denotes the difficulty of the problem that Mr. B should choose.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
5 3 2 4 1
3
1 3
2 4
3 5
5
10 6 4 8 2
3
1 3
2 4
3 5

<strong>Output:</strong>
Case 1:
3
3
2
Case 2:
6
6
4
</pre>