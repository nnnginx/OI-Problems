<p>As you might already know, Ada the Ladybug is a farmer. She grows many beautiful flowers. Each of the flowers has something called "blooming value".  As long as <strong> A<sub>i</sub> &lt; A<sub>i</sub> </strong>¨’<strong> A<sub>j</sub> &lt;     A<sub>j</sub> </strong> (where ¨’ stands for binary XOR, and <strong>A</strong> stands for "blooming value") is true for any pair of flowers (in any order), then those flowers-pair might bloom into a wonderful blossom, if they are replanted into same box (at most 2 flowers can be put into one box).</p>
<p>Ada wants to maximize the number of blossoms - can you find it?</p>
<h3>Input</h3>
<p>The first line of input containt <strong>1 ¡Ü T ¡Ü 500 </strong> test-cases.</p>
<p>The first line of each test-case contains <strong> N 1 ¡Ü N     ¡Ü 5000</strong></p>
<p>The next line contains <strong>N</strong> integers <strong>0 &lt; A<sub>i</sub> ¡Ü     10<sup>18</sup></strong>, the blooming value of flower.</p>
<p><strong>NOTE:</strong> The number of test-cases varies depending on size of array (the longest array won't be a single file more than once).</p>
<h3>Output</h3>
<p>For each test-cases, print the maximal number of blossoms Ada can achieve.</p>
<h3>Example Input 1</h3>
<pre>6
7
8 5 4 8 4 9 11
6
9 9 12 12 4 6
3
7 7 4
4
10 6 9 1
8
11 4 12 3 1 2 1 10
4
12 2 5 2
</pre>
<h3>Example Output 1</h3>
<pre>0
2
0
1
4
1
</pre>
<h3>All possible pairs 1</h3>
<pre>Test-case 1:
Test-case 2:
4 &lt; 8 &lt; 12
4 &lt; 8 &lt; 12
6 &lt; 10 &lt; 12
6 &lt; 10 &lt; 12
Test-case 3:
Test-case 4:
1 &lt; 8 &lt; 9
Test-case 5:
1 &lt; 2 &lt; 3
1 &lt; 10 &lt; 11
1 &lt; 2 &lt; 3
1 &lt; 10 &lt; 11
2 &lt; 8 &lt; 10
2 &lt; 9 &lt; 11
3 &lt; 9 &lt; 10
3 &lt; 8 &lt; 11
4 &lt; 8 &lt; 12
Test-case 6:
5 &lt; 9 &lt; 12
</pre>
<h3>Example Input 2</h3>
<pre>1
20
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20
</pre>
<h3>Example Output 3</h3>
<pre>7
</pre>