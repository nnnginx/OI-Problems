<p>Ada the Ladybug owns a beautiful field where she grows vegetables. She often visits local Farmers Market, where she buys new seeds. Since two types of vegetable can't share same field, she always divide the field, by either vertical or horizontal line (she is very precise, so the width of line is negligible). Since she visits Farmers Market almost every day, she has already made a lot of such lines, so she needs your help with finding out the area of biggest field.</p>
<h3>Input</h3>
<p>The first line will contain <strong>0 &lt; T ¡Ü 200</strong>, the number of test-cases.</p>
<p>Then <strong>T</strong> test-cases follow, each beginning with three integers <strong> 1     ¡Ü N,M ¡Ü 2*10<sup>9</sup></strong>, <strong>1 ¡Ü Q ¡Ü 10<sup>5</sup></strong>, top right corner of field (field goes from <strong>[0,0]</strong> to <strong>[N,M]</strong>) and number of field divisions.</p>
<p>Afterward <strong>Q</strong> lines follows:</p>
<p><strong>0 x (0 ¡Ü x ¡Ü N)</strong>, meaning that line was made vertically, on coordinate <strong>x</strong></p>
<p><strong>1 y (0 ¡Ü y ¡Ü M)</strong>, meaning that line was made horizontally, on coordinate <strong>y</strong></p>
<p>Sum of <strong> Q </strong> over all test-cases won't exceed <strong>10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>Print <strong>Q</strong> lines, the area of biggest field after each line was made.</p>
<h3>Example Input</h3>
<pre>2
10 10 5
0 5
0 8
1 1
1 9
1 5
10 10 5
0 5
1 4
1 6
1 8
0 5
</pre>
<h3>Example Output</h3>
<pre>50
50
45
40
20
50
30
20
20
20
</pre>