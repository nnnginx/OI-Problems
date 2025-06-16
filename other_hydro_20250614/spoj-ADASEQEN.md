<p>Ada the Ladybug has two string which she wants to give to her friends. As she doesn't want to distinguish between them, she wants to use only some common subsequence. Firstly she wanted to simply use the longest common subsequence but then she realized it wouldn't be <em>kosher</em>.</p>
<p>She assigned a positive value to each letter. Now she wants to find the most expensive subsequence.</p>
<h3>Input</h3>
<p>The first line of each test-case will contain two integers <strong>1 ¡Ü N, M ¡Ü     2000</strong>, the length of each subsequence.</p>
<p>The next line will contain <strong>26</strong> integers (<strong>1 ¡Ü P<sub>i</sub> ¡Ü     10<sup>5</sup></strong>), the price of each letter.</p>
<p>The next line will contain string of length <strong>N</strong> consisting of lowercase english alphabet.</p>
<p>The next line will contain string of length <strong>M</strong> consisting of lowercase english alphabet.</p>
<h3>Output</h3>
<p>For each test-case, print the cost of the most expensive common subsequence.</p>
<h3>Example Input</h3>
<pre>4 4
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
abcd
dbca
</pre>
<h3>Example Output</h3>
<pre>2
</pre>
<h3>Example Input</h3>
<pre>3 3
1 7 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
baa
aab
</pre>
<h3>Example Output</h3>
<pre>7
</pre>
<h3>Example Input</h3>
<pre>4 5
1 4 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 6
zbbz
bbzbb
</pre>
<h3>Example Output</h3>
<pre>14
</pre>
<h3>Example Input</h3>
<pre>3 3
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
abc
def
</pre>
<h3>Example Output</h3>
<pre>0
</pre>