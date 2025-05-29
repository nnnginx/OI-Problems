<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Consider a string S, consisting of only lowercase alphabets.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given a list of queries, each containing a non-empty string STR.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each query, you have to output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Among all substrings of S, the next lexicographically greater substring after STR.</div>
<p>Consider a string <strong>S</strong>, consisting of only lowercase alphabets.</p>
<p>You are given a list of queries, each containing a non-empty string <strong>STR</strong>.</p>
<p>For each query, you have to output:</p>
<p>Among all substrings of S, the next lexicographically greater substring after STR.</p>
<p><span style="font-size: small;">Note: If no such substring of S exists which is lexicographically greater than STR, output -1.</span></p>
<p><strong>Constraints:</strong></p>
<p>1&lt;=|S|&lt;=10^5</p>
<p>1&lt;= Q &lt;=10^5</p>
<p>1&lt;=|STR|&lt;=10^5</p>
<p>summation of |STR| for all Q &lt;=10^5</p>
<p><span style="font-size: 1.17em;"><strong>Input</strong></span></p>
<p>First line contains the string<strong> S</strong>.</p>
<p>The next line contains <strong>Q</strong>, the number of Queries to answer.</p>
<p>The next Q lines contain <strong>STR </strong>for each query.</p>
<h3>Output</h3>
<p>Output the answer for each query in a new line.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>dabab<br>3<br>ab<br>abaa<br>bab<br><span style="font-weight: bold;">Output:<br></span>aba<br>abab<br>d</pre>
<pre><span style="font-size: 10.3999996185303px; font-weight: bold;">Input:<br></span><span style="font-size: 10.3999996185303px;">a<br></span><span style="font-size: 10.3999996185303px;">1<br></span><span style="font-size: 10.3999996185303px;">a<br></span><span style="font-size: 10.3999996185303px; font-weight: bold;">Output:<br></span><span style="font-size: 10.3999996185303px;">-1</span></pre>