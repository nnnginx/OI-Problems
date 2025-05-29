<p>One day Blue Mary goes to a nearby supermarket to buy some goods. She has a backpack, whose capacity is <i>V-Max</i>. She finds that there are many goods in the market, each has a volume <i>V<sub>i</sub></i>(it will always be a multiple of 10 and less than 10000) and an importance <i>C<sub>i</sub></i>(1&lt;= <i>C<sub>i</sub></i> &lt;=5). Since she has almost unlimited money, the only problem she is to solve is how to choose goods such that the total volume won't exceed the capacity of the backpack and the sum of the product of the volume and the importance of each good is maximum. To be an excellent mathematician, she comes up with the answer quickly, and now she wants you to do a harder task. There are two kinds of goods: main goods and attachments. If you want to buy an attachment you must buy its main good before.</p>
<h3>Input</h3>
<p>Multiple test cases, the number of them is given in the very first line.</p>
<p>For each test case:</p>
<p>The first line contains two space-separated integers <i>V-Max</i> (1&lt;=<i>V-Max</i>&lt;=32000) and the number of the goods <i>N</i> (1&lt;=<i>N</i>&lt;=60). N lines follow, each contains three space-separated integers <i>V<sub>i</sub></i>, <i>C<sub>i</sub></i> and a integer <i>u</i>. If <i>u</i> is not 0, this good is an attachment of good <i>u</i>(as the order in the input file).</p>
<p>To make the problem not too difficult, Blue Mary tells you that:</p>
<p>(A) An attachment won't have any attachments which belong to it.</p>
<p>(B) A main good will always have less than 3 attachments.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>The first and the only line contains a single integer denoted the answer.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
1000 5
800 2 0
400 5 1
300 5 1
400 3 0
500 2 0

<b>Output:</b>
2200
</pre>