<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Two functions f and g (f, g: X → X) are commuting if and only if f(g(x)) = g(f(x)) for each x in X.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For example, functions f(x) = x + 1 and g(x) = x − 2 are commuting, whereas functions f(x) = x + 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and g(x) = 2x are not commuting.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each function h (h: N_n → N_n, where N_n = 1, 2, ..., n and n is positive integer) can be represented as a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">value list — a list in which the i-th element is equal to h(i). For example, a function h(x) = ceil(x/2) from</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">N_5 to N_5 has the value list [1, 1, 2, 2, 3].</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The value lists are ordered lexicographically: list [a1 ... an] is smaller than list [b1 ... bn] if and only if</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">there exists such an index k that a_k &lt; b_k, and a_l = b_l for any index l &lt; k.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The function f (f: X → X) is bijective if for every y in X, there is exactly one x in X such that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">f(x) = y.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given a bijective function f (f: N_n → N_n, n is positive integer), find the function g that is commuting</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">with f and has the lexicographically smallest possible value list.</div>
<p>&nbsp;</p>
<p>Two functions f and g (f, g: X → X) are commuting if and only if f(g(x)) = g(f(x)) for each x in X.&nbsp;For example, functions f(x) = x + 1 and g(x) = x − 2 are commuting, whereas functions f(x) = x + 1&nbsp;and g(x) = 2x are not commuting.</p>
<p>&nbsp;</p>
<p>Each function h (h: N<sub>n</sub> → N<sub>n</sub>, where N<sub>n</sub> = {1, 2, ..., n} and n is positive integer) can be represented as a&nbsp;value list — a list in which the i-th element is equal to h(i). For example, a function h(x) = ceil(x/2) from&nbsp;N<sub>5</sub> to N<sub>5</sub> has the value list [1, 1, 2, 2, 3].</p>
<p>&nbsp;</p>
<p>The value lists are ordered lexicographically: list [a<sub>1</sub> ... a<sub>n</sub>] is smaller than list [b<sub>1</sub> ... b<sub>n</sub>] if and only if&nbsp;there exists such an index k that a<sub>k</sub> &lt; b<sub>k</sub>, and a<sub>l</sub> = b<sub>l</sub> for any index l &lt; k.</p>
<p>&nbsp;</p>
<p>The function f (f: X → X) is bijective if for every y in X, there is exactly one x in X such that&nbsp;f(x) = y.</p>
<p>&nbsp;</p>
<p>Given a bijective function f (f: N<sub>n</sub> → N<sub>n</sub>, n is positive integer), find the function g that is commuting&nbsp;with f and has the lexicographically smallest possible value list.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input file contains the number of test cases. Each test case is described by a line containing a single integer number n — the number of the elements in the value list of a bijective function f (1 ≤ n ≤ 200000), followed by another line which contains the value list of the function f.</p>
<h3>Output</h3>
<p>For each test case, output a single line containing n integer numbers — the value list of function g that commutes with the function f and has the lexicographically smallest value list.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10
1 2 3 4 5 6 7 8 9 10
10
2 3 4 5 6 7 8 1 9 10

<strong>Output:</strong>
1 1 1 1 1 1 1 1 1 1
1 2 3 4 5 6 7 8 9 9<span style="white-space: normal;">
</span></pre>