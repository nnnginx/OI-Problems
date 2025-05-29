<p>Ada the Ladybug had a lecture about algorithms. She learned that sorting can be done in O(NlogN) time. She also learned concept of <strong>stable sort</strong>. For those who missed the lecture, it means that as long as there are two equal elements in the array their mutual position <strong>won't</strong> change after the sort.</p>
<p>Ada wanted to come up with something new, so she proposed <strong>unstable     sort</strong>. It is sort with following property: "As long as there are two equal elements in the array their mutual position <strong>will</strong> change after the sort".</p>
<p>As Ada has only theoretical knowledge about it, she has asked you to construct such algorithm for her.</p>
<h3>Input</h3>
<p>The first line of each test-case will contain an integer <strong>1 ¡Ü N ¡Ü     10<sup>5</sup></strong>, the length of an array.</p>
<p>The next line will contain <strong>N</strong> integers <strong>1 ¡Ü A<sub>i</sub> ¡Ü     10<sup>5</sup></strong>, the elements of the array.</p>
<h3>Output</h3>
<p>For each test-case, print <strong>N</strong> numbers, the indexes of each element on which it was in original array. Indexes start with <strong>1</strong>.</p>
<h3>Example Input</h3>
<pre>4
1 2 3 4
</pre>
<h3>Example Output</h3>
<pre>1 2 3 4
</pre>
<h3>Example Input</h3>
<pre>3
3 2 1
</pre>
<h3>Example Output</h3>
<pre>3 2 1
</pre>
<h3>Example Input</h3>
<pre>6
6 6 6 6 6 6
</pre>
<h3>Example Output</h3>
<pre>6 5 4 3 2 1
</pre>
<h3>Example Input</h3>
<pre>5
5 5 2 2 3
</pre>
<h3>Example Output</h3>
<pre>4 3 5 2 1
</pre>
<h3>Example Input</h3>
<pre>6
1 2 1 2 1 2
</pre>
<h3>Example Output</h3>
<pre>5 3 1 6 4 2
</pre>