<p>Ada the Ladybug is already planning her birthday party. It is not an easy process since she has many friends. At first, she had a plan to invite only subset of her friends but now her plans are different. She wants to satisfy all her friends so she is going to hold multiple parties. Anyway she wants to satisfy fact, that each of her friends will have all of their friends at the same party while there will be no one, who is not his/her friend.</p>
<p>Problem is, that with current layout, it might not be possible. It is not so easy to let two bugs become friend, and it is not so "nice" to make them enemies... yet both are possible. Ada asked you to find the minimal number of such operations so that the parties will be possible! Ada doesn't want to do many of such operations so she already made a little research and found out she won't need more than <strong>12</strong> such operations.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong> 1 ¡Ü T ¡Ü 100</strong>, the number of test-cases.</p>
<p>The first line of each test-case begins with <strong>1 ¡Ü N ¡Ü 62</strong>, the number of her friends.</p>
<p>Each of next <strong>N</strong> lines contain <strong>N</strong> integers <strong>A<sub>i,j</sub></strong> (either <strong>0</strong> or <strong>1</strong>), where <strong>1</strong> means the <strong>i<sup>th</sup></strong> friend likes <strong>j<sup>th</sup></strong> (and <strong>0</strong> means the opposite)</p>
<p>Note, that the matrix will be symmetrical.</p>
<p>Each insect is friend with itself!</p>
<h3>Output</h3>
<p>For each test-case output the minimal number of introductions and antagonizations.</p>
<h3>Example Input</h3>
<pre>7
7
1 0 0 0 0 0 0
0 1 1 1 0 0 0
0 1 1 0 0 0 1
0 1 0 1 1 1 0
0 0 0 1 1 1 0
0 0 0 1 1 1 0
0 0 1 0 0 0 1
8
1 1 1 0 0 0 1 1
1 1 1 0 0 0 0 1
1 1 1 0 0 0 0 0
0 0 0 1 1 0 0 0
0 0 0 1 1 1 0 0
0 0 0 0 1 1 0 0
1 0 0 0 0 0 1 1
1 1 0 0 0 0 1 1
8
1 0 0 0 0 0 0 0
0 1 1 0 0 0 0 1
0 1 1 0 0 0 0 0
0 0 0 1 0 0 0 0
0 0 0 0 1 1 1 0
0 0 0 0 1 1 1 0
0 0 0 0 1 1 1 0
0 1 0 0 0 0 0 1
3
1 0 0
0 1 0
0 0 1
7
1 1 0 0 0 1 0
1 1 0 0 1 0 1
0 0 1 1 0 0 1
0 0 1 1 0 0 0
0 1 0 0 1 0 0
1 0 0 0 0 1 1
0 1 1 0 0 1 1
6
1 1 1 0 0 0
1 1 1 0 1 1
1 1 1 0 0 0
0 0 0 1 0 0
0 1 0 0 1 1
0 1 0 0 1 1
5
1 1 1 1 1
1 1 1 1 0
1 1 1 0 1
1 1 0 1 1
1 0 1 1 1
</pre>
<h3>Example Output</h3>
<pre>2
4
1
0
4
2
2
</pre>