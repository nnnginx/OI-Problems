<p>You are given a sequence of <strong>n</strong> integers <strong>a<sub>0</sub>, a<sub>1</sub>, ..., a<sub>n-1</sub></strong>. You are also given several queries consisting of indices <strong>i</strong> and <strong>j</strong> (<em>0 ¡Ü i ¡Ü j ¡Ü n-1</em>). For each query, determine the number of occurrences of the most frequent value among the integers <strong>a<sub>i</sub>, ..., a<sub>j</sub></strong>.</p>
<h3>Input</h3>
<p>First line contains two integers <strong>n</strong> and <strong>q</strong> (<em>1 ¡Ü n, q ¡Ü 100000</em>). The next line contains <strong>n</strong> integers <strong>a<sub>0</sub>, ... ,a<sub>n-1</sub></strong> (<em>0 ¡Ü a<sub>i</sub> ¡Ü 100000</em>, for each <em>i ¡Ê {0, ..., n-1}</em>) separated by spaces. The following <strong>q</strong> lines contain one query each, consisting of two integers <strong>i</strong> and <strong>j</strong> (<em>0 ¡Ü i ¡Ü j ¡Ü n-1</em>), which indicates the boundary indices for the query.</p>
<h3>Output</h3>
<p>For each query, print one line with one integer: The number of occurrences of the most frequent value within the given range.</p>
<h3>Example</h3>
<pre><strong>Input:<br><br></strong>5 3<br>1 2 1 3 3<br>0 2<br>1 2<br>0 4

<strong>Output:</strong>
<br>2<br>1<br>2<br><br>NOTE - This problem is similar to a problem Frequent values.</pre>