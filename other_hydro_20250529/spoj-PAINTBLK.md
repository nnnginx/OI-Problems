<p><i>n</i> blocks are put in a line. You have <i>k</i>(1&lt;=<i>k</i>&lt;=15) kinds of dope, the <i>i</i>-th dope is enough to paint c<sub>i</sub> (1&lt;=c<sub>i</sub>&lt;=5) blocks. You may assume the sum of all the c<sub>i</sub> equals to <i>n</i>. Your task is to calculate the number of ways to paint the blocks with these kinds of dope, such that no two adjacent blocks are painted with the same kind of dope.</p>
<h3>Input</h3>
<p>Ten test cases(given one after another, you have to process all!). For each test case, the first line contains an integer <i>k</i>, the second line contains <i>k</i> integers, c<sub>1</sub>, c<sub>2</sub>, ...c<sub>k</sub>.</p>
<h3>Output</h3>
<p>Ten lines, each contains an integer, the number of ways modulo 1000000007.</p>
<h3>Example</h3>
<pre><b>Input:</b>
3
1 2 3
5
2 2 2 2 2
10
1 1 2 2 3 3 4 4 5 5
[and 7 test cases more]

<b>Output:</b>
10
39480
85937576
[and 7 test cases more]
</pre>