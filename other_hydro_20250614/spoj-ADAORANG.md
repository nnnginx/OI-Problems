<p>Ada the Ladybug lives near an orange tree. Instead of reading books, she investigates the oranges. The oranges on orange tree can be in up to 5*50 Shades of Orange. She walks from orange to orange, examining different properties of orange tree. The oranges are connected by branches. There is more oranges then branches, yet it is still possible to get from any orange to any other orange [through branches]. The tree is rooted.</p>
<p>Ada has many questions in following form: She goes from orange <strong>A</strong> to orange <strong>B</strong> (by shortest path) and is interested in total number different Shades of Orange among all subtrees of all edges on shortest path.</p>
<h3>Input</h3>
<p>The first line of input consists of <strong>1 ¡Ü T ¡Ü 100</strong>, the number of test-cases.</p>
<p>The first line of each test case contains three integers <strong>1 ¡Ü N, Q ¡Ü     4.5*10<sup>5</sup>, 0 ¡Ü R &lt; N</strong>, the number of oranges, the number of questions and number of root.</p>
<p>Next line contains <strong> N </strong> integers <strong>1 ¡Ü S<sub>i</sub> ¡Ü     250</strong>, the shade of orange of orange <strong>i</strong>.</p>
<p>Next <strong>N-1</strong> lines contains two integers <strong>0 ¡Ü I, J &lt; N, I ¡Ù J </strong>, the numbers of oranges which are connected by branch.</p>
<p>Next <strong>Q</strong> lines contains two integers <strong>0 ¡Ü A, B &lt; N</strong>, the path Ada is interested about.</p>
<p>The sum of all <strong>N</strong> and all <strong>Q</strong> among all test-cases won't exceed <strong>10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>For each question answer the number of shades in all subtrees of all nodes on shortest path from <strong>A</strong> to <strong>B</strong>.</p>
<h3>Example Input</h3>
<pre>1
10 7 1
1 2 1 4 5 6 6 8 9 9
0 9
9 3
3 4
4 6
4 5
4 8
1 3
1 2
2 7
4 4
8 6
0 6
7 0
7 2
0 0
2 3
</pre>
<h3>Example Output</h3>
<pre>3
3
5
7
2
1
7
</pre>
<h3>Explanation - shades in subtrees</h3>
<pre>5 6 9
5 6 9
1 4 5 6 9
1 2 4 5 6 8 9
1 8
1
1 2 4 5 6 8 9
</pre>