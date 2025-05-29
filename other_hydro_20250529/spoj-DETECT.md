<p>E.T. Inc. employs Maryanna as alien signal researcher. To identify possible alien signals and background noise, she develops a method to evaluate the signals she has already received. The signal sent by E.T is more likely regularly alternative.</p>
<p>Received signals can be presented by a string of small latin letters 'a' to 'z' whose length is <strong>N</strong>. For each <em>X</em> between 1 and <strong>N</strong> inclusive, she wants you to find out the maximum length of the substring which can be written as a concatenation of <em>X</em> same strings. For clarification, a substring is a consecutive part of the original string.</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong>, the number of test cases (<strong>T</strong> &lt;= 200). Most of the test cases are relatively small. <strong>T</strong> lines follow, each contains a string of only small latin letters 'a' - 'z', whose length <strong>N</strong> is less than 1000, without any leading or trailing whitespaces.</p>
<h3>Output</h3>
<p>For each test case, output a single line, which should begin with the case number counting from 1, followed by <strong>N</strong> integers. The <em>X</em>-th (1-based) of them should be the maximum length of the substring which can be written as a concatenation of <em>X</em> same strings. If that substring doesn't exist, output 0 instead. See the sample for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
arisetocrat
noonnoonnoon

<strong>Output:</strong>
Case #1: 11 0 0 0 0 0 0 0 0 0 0
Case #2: 12 8 12 0 0 0 0 0 0 0 0 0
</pre>
<h3>Hint</h3>
<p>For the second sample, the longest substring which can be written as a concatenation of 2 same strings is "noonnoon", "oonnoonn", "onnoonno", "nnoonnoo", any of those has length 8; the longest substring which can be written as a concatenation of 3 same strings is the string itself. As a result, the second integer in the answer is 8 and the third integer in the answer is 12.</p>