<p>Protocol is really weird in Byteland. For instance, it is required that, when presenting arms before an officer, soldiers should stand in a single row (at positions numbered from 1 to <i>n</i>). Soldiers may have one of 4 possible ranks, distinguished by the number of squiggles on the epaulets (between 1 and 4). Soldiers standing beside each other must have a difference in rank of at least two squiggles. Moreover, there are additional sets of rules (different for every province). Each rule states that soldiers standing at some given positions of the row must differ in rank by at least a squiggle.
</p><p>Starting from the new year onwards, some provinces are changing their set of protocol rules. As the Senior Military Secretary of Protocol, it is your task to approve the new rules. To your surprise, some of the provinces have put forward protocol rules which are quite impossible to fulfill, even if the soldiers were to be specially selected for the purpose of presenting arms. Detect all such offending provinces and on no account approve their laws.

</p><h3>Input</h3>
<p>The first line of input contains a single positive integer <i>t</i>&lt;=10 - the number of provinces which are proposing new laws. <i>t</i> sets of rules follow, separated by empty lines.
</p><p>
Each set of rule begins with a line containing two non-negative integers <i>n</i> <i>p</i> (<i>n</i>&lt;=100000, <i>p</i>&lt;=100000) - the number of soldiers arranged and the number of rules proposed in the province, respectively. Each of the next <i>p</i> lines contains a single rule: an integer <i>b<sub>i</sub></i> (2&lt;=<i>b<sub>i</sub></i>&lt;=<i>n</i>), followed by <i>b<sub>i</sub></i> integers <i>a</i><sub>1</sub>,<i>a</i><sub>2</sub>,...,<i>a<sub>bi</sub></i> (1&lt;=<i>a<sub>k</sub></i>&lt;=<i>n</i>). Such a rule means that soldiers standing at positions <i>a</i><sub>1</sub>,<i>a</i><sub>2</sub>,...,<i>a<sub>bi</sub></i> must all be of different rank.

</p><h3>Output</h3>
<p>For every set of rules presented at input, output a single line containing the word <tt><i>rejected</i></tt> if no unit of soldiers can be arranged in accordance with protocol, or the word <tt><i>approved</i></tt> in the opposite case.

</p><h3>Example</h3>

<pre><b>Input:</b>
2

2 1
2 1 2

5 2
3 1 3 2
4 2 3 4 5

<b>Output:</b>
approved
rejected
</pre>