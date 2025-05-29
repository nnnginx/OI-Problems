<p>Anyone that ever went to men's restroom knows about International Choice of Urinal Protocol. It reads as follows:</p>
<p><em>This protocol specifies the rules of choosing a urinal, for a given row of urinals (some of them may be already taken).</em></p>
<ul>
<em>
<li>One should choose a urinal that maximizes the distance to the closest urinal that is already taken.</li>
<li>If there is more than one urinal satisfying the condition above, one should choose a urinal that is the farthest from the door.</li>
<li>One must not take a urinal that is adjacent to an already taken urinal. This rule is introduced in order to avoid Awkwardness.</li>
</em>
</ul>
<p>There is a row of <strong>n</strong> urinals, numbered with consecutive integers, from left to right, starting with 1. The door is located to the right of the urinal number <strong>n</strong>. At first, the restroom is empty. Let's assume that people are coming in, one by one, taking the urinals according to the Protocol, without freeing them up in the meantime. Which urinal will be chosen by the <strong>k</strong>-th person?</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, testcases follow.</p>
<p>One testcase is a single line, containing two natural numbers <strong>n</strong> and <strong>k</strong>.</p>
<p>(1 &lt;= <strong>k</strong> &lt;= <strong>n</strong> &lt;= 10<sup>18</sup>)</p>
<h3>Output</h3>
<p>For every testcase you should print one line containing the number that corresponds to a urinal taken by the <strong>k</strong>-th person coming to the restroom with <strong>n</strong> urinals. If there is no way for that person to pick a urinal without violating the Protocol, you should print "OOPS" instead.</p>
<h3>Example</h3>
<p>Input:</p>
<pre>10
5 1
5 2
5 3
5 4
5 5
9 5
9 6
19 8
23 6
27 12
</pre>
<p>Output:</p>
<pre>1
5
3
OOPS
OOPS
7
OOPS
12
9
OOPS
</pre>