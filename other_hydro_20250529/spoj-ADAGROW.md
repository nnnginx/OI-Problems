<p>As you might already know, Ada the Ladybug is a farmer. She grows vegetables. At the moment, all her vegetables are in one furrow. She is going to replant them into a few new furrows (while keeping the order of the vegetables).</p>
<p>The total cost of growing the vegetables will be equal to the sum of absolute differences between neighboring vegetables. Ada wants to minimize the cost, can you help her?</p>
<h3>Input</h3>
<p>The first line of input containt <strong>1 ¡Ü T ¡Ü 500 </strong> test-cases.</p>
<p>The first line of each test-case contains two integers <strong> N, K 1 ¡Ü N     ¡Ü 2000, 1 ¡Ü K ¡Ü 20</strong></p>
<p>The next line contains <strong>N</strong> integers <strong>0 ¡Ü A<sub>i</sub> &lt;     10<sup>4</sup></strong>, the costs of vegetables.</p>
<p><strong>NOTE:</strong> The number of test-cases varies depending on size of array (the longest array won't be a single file more than once).</p>
<h3>Output</h3>
<p>For each test-cases, print the minimal costs.</p>
<h3>Example Input</h3>
<pre>5
4 2
1 2 5 6
5 1
1 2 5 7 11
6 3
1 3 1 3 1 3
8 2
1 6 2 5 1 6 2 5
5 3
1 9 15 4 11
</pre>
<h3>Example Output</h3>
<pre>2
10
0
6
5
</pre>
<h3>Additional Information</h3>
<pre>TEST-CASE-1:
1 2
5 6
TEST-CASE-2:
1 2 5 7 11
TEST-CASE-3:
1 1 1
3 3 3

TEST-CASE-4:
1 2 1 2
6 5 6 5
TEST-CASE-5:
1 4
9 11
15
</pre>
<h3>Example Input 2</h3>
<pre>1 
7 2 
2 5 7 4 8 8 4 
</pre>
<h3>Example Output 2</h3>
<pre>5
</pre>
<h3>Example Input 3</h3>
<pre>1
10 2
4 5 4 3 4 3 2 3 2 3
</pre>
<h3>Example Output 3</h3>
<pre>4
</pre>