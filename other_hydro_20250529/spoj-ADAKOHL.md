<p>As you might already know, Ada the Ladybug is a farmer. She has a garden with kohlrabi. Each kohlrabi has assigned a quality, which is a number (possibly negative, since the kohlrabi might be rotten).</p>
<p>Ada wants to gather some kohlrabi so she wants to pick a line such that the sum of kohlrabi on the line is maximal. Can you help her to find such line?</p>
<h3>Input</h3>
<p>The first line of input containts  <strong>1 ¡Ü T ¡Ü 100 </strong>, the number of test-cases (anyway note that for biggest test-cases there will be only 1 test-case).</p>
<p>The first line of each test-case contains <strong> 0 &lt; N ¡Ü 3000 </strong>, the number of kohlrabi.</p>
<p>The next <strong> N </strong> lines contains three integers <strong>x, y, q:     -10<sup>9</sup> ¡Ü x, y     ¡Ü 10<sup>9</sup>, -10<sup>4</sup> ¡Ü q ¡Ü 10<sup>4</sup></strong>, the coordinates of kohlrabi and its quality (note that no two kohlrabil will grow on same coordinates).</p>
<h3>Output</h3>
<p>For each test-case, print the best achieavable sum of qualities of kohlrabies on a single line.</p>
<h3>Example Input</h3>
<pre>5
4
0 0 1
1 1 1
2 2 1
3 3 1
5
0 0 -10
1 0 2
0 1 3
-1 0 2
0 -1 3
3
0 0 -1
1 1 -2
1 3 -5
2
0 0 666
1 7 -666
5
0 0 1
99999999 0 6
0 99999999 5
-99999999 0 6
0 -99999999 5
</pre>
<h3>Example Output</h3>
<pre>4
5
0
666
13
</pre>
<h3>Example Input 2</h3>
<pre>1
7
10 8 -2
9 4 -1
-3 -5 -5
7 5 1
-3 2 -6
5 10 -4
9 7 10
</pre>
<h3>Example Output 2</h3>
<pre>10
</pre>
<h3>Example Input 3</h3>
<pre>1
4
-6 0 9
7 4 7
7 -6 -10
-6 7 10
</pre>
<h3>Example Output 3</h3>
<pre>19
</pre>
<h3>Example Input 4</h3>
<pre>1
6
-10 -1 -10
8 3 4
0 9 -2
4 -6 1
6 0 10
-6 1 -10
</pre>
<h3>Example Output 4</h3>
<pre>14
</pre>