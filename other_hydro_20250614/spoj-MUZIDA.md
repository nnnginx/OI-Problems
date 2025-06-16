<p>Given a string <b>S</b> of lowercase Latin letters. You are to answer <b>Q</b> queries: given <i>l</i> and <i>r</i> (1 &lt;= <i>l</i> &lt;= <i>r</i> &lt;= |<b>S</b>|), count the number of distinct non-empty subsequences of the substring <b>S</b>[<i>l</i>..<i>r</i>].</p>

<h3>Input</h3>
<p>Multiple test cases. For each test case:</p>

<p>The first line of input contains a string <b>S</b>.(|<b>S</b>| &lt;= 40000). The second line contains a single integer <b>Q</b> (<b>Q</b>&lt;= 100000).  <b>Q</b> lines follow, each contains two space separated integers <i>l</i> and <i>r</i>.</p>

<p>Input terminates by EOF.</p>
<p>Input data is almost uniformly-random generated, the number of "large" test cases is relatively small.</p>

<h3>Output</h3>
<p>For each query output one line - the answer, modulo 10<sup>9</sup> + 2015.

</p><h3>Example</h3>
<pre><b>Input:</b>
aabababb
5
1 8
1 4
3 5
5 7
3 8
aaccbb
5
1 6
3 4
2 5
1 4
3 6

<b>Output:</b>
63
9
6
6
27
26
2
11
8
8
</pre>