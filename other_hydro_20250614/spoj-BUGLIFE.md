<p>Professor Hopper is researching the sexual behavior of a rare species of bugs. He assumes that
they feature two different genders and that they only interact with bugs of the opposite gender. In
his experiment, individual bugs and their interactions were easy to identify, because numbers were
printed on their backs.<br><br>
Given a list of bug interactions, decide whether the experiment supports his assumption of two
genders with no homosexual bugs or if it contains some bug interactions that falsify it.</p>

<h3>Input</h3>
<p>The first line of the input contains the number of scenarios. Each scenario starts with one line
giving the number of bugs (at least one, and up to 2000) and the number of interactions (up to
1000000) separated by a single space. In the following lines, each interaction is given in the form of
two distinct bug numbers separated by a single space. Bugs are numbered consecutively starting
from one.</p>

<h3>Output</h3>
<p>The output for every scenario is a line containing ¡°<tt>Scenario #i:</tt>¡±, where i is the number of the
scenario starting at 1, followed by one line saying either ¡°<tt>No suspicious bugs found!</tt>¡± if the
experiment is consistent with his assumption about the bugs¡¯ sexual behavior, or ¡°<tt>Suspicious
bugs found!</tt>¡± if Professor Hopper¡¯s assumption is definitely wrong.</p>

<h3>Example</h3>
<pre><b>Input:</b>
2
3 3
1 2
2 3
1 3
4 2
1 2
3 4

<b>Output:</b>
Scenario #1:
Suspicious bugs found!
Scenario #2:
No suspicious bugs found!</pre>