<p>If x = a<sub>0</sub>a<sub>1</sub>a<sub>2</sub>...a<sub>n-1</sub> is a string where a<sub>i</sub> denotes the character at index i, a subsequence a<sub>j0</sub>a<sub>j1</sub>a<sub>j2</sub>...a<sub>jn</sub> is called an upsubsequence if a<sub>j0</sub> &lt;= a<sub>j1</sub> &lt;= a<sub>j2</sub> &lt;= ... &lt;= a<sub>jn</sub> and j0 &lt; j1 &lt; j2 &lt; ... &lt; jn.</p>

<p>A maximal upsubsequence of a string is defined as the upsubsequence of maximum length.  BuggyD observes that a string <b>x</b> can have many maximal upsubsequences.  Help him find all the maximal upsubsequences in <b>x</b>.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>Each test case consists of a single line containing a string <b>x</b>, where the length of <b>x</b> is no more than 100.  <b>x</b> will not contain any spaces, tabs or other whitespace characters.</p>

<h3>Output</h3>
<p>For each test csae, output all of the maximal upsubsequences of <b>x</b> in lexicographical order.  Print a blank line after each test case.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
abcbcbcd

<b>Output:</b>
abbbcd
abbccd
abcccd
</pre>