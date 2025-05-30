<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Many centuries later lawyers discovered that there were only two types of laws in the kingdom:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">² direct law, that states a new norm;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">² canceling law, that cancels one of the previous laws.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The law is considered active if and only if there is no active law that cancels it.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are to write program that ¯nds out which laws are still active.</div>
<p>Long ago, in a kingdom far, far away the king decided to keep a record of all laws of his kingdom. From that moment whenever a new law was passed, a corresponding record was added to the law archive.</p>
<p>Many centuries later lawyers discovered that there were only two types of laws in the kingdom:</p>
<ul>
<li>direct law, that states a new norm;</li>
<li>canceling law, that cancels one of the previous laws.</li>
</ul>
<p>The law is considered active if and only if there is no active law that cancels it.</p>
<p>You are to write program that finds out which laws are still active.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input contains T, the number of test cases. T test cases follow.</p>
<p>The first line of each test case contains an integer number n (1 &lt;= n &lt;= 100000) - the number of passed laws.</p>
<p>The following n lines describe one law each. Each description has one of the following formats:</p>
<ul>
<li>"declare", meaning that a direct law was passed.</li>
<li>"cancel i", where i is the number of law being cancelled by this one.</li>
</ul>
<p>The laws are numbered from one.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case your output must contain a line with the number of active laws. The following line must contain numbers of these laws listed in increasing order.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5
declare
cancel 1
declare
cancel 2
cancel 3

<strong>Output:</strong>
3
1 4 5</pre>