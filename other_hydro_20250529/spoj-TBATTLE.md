<p>Thor is caught up in a fierce battle with Loki's army. This army consists of frost giants that have magical powers with   them. Their strength levels gets multiplied when they are together. Giants are not highly skilled in the arts of   combat, but their sheer size and strength make them formidable opponents even for the Asgardian gods. Thor is no exception. They recover very fast from physical injury but their recovery slows down when they are exposed to   extreme heat. <br> Thor's hammer can generate heat only in multiples of heat quantum <strong>N</strong>. Frost giants get killed only   when their combined strength level is exactly equal to the heat level of the hammer. Thor is interested in killing a   continuous stretch of frost enemies with a throw of his hammer with a preference to kill closer enemies first.<br> <strong>Continuous stretch</strong> is defined as a set of consecutive elements.<br> Help   Thor to determine the minimum stretch of frost giants that could be killed in a throw. In case of multiple minimal   stretches, output the indices of that stretch that has lowest starting index. If there is no such continuous stretch   possible then print -1.</p>
<h3>Input</h3>
<p>The first line will contain <strong>N</strong>, the number of Frost Giants in Loki's army and the Heat quantum.<br> The second line will contain <strong>N</strong> integers<strong> (a_0, a_2....., a_n-1)</strong> -  the strength of each frost giant. <br> Minimum stretch of the army should be 1.</p>
<ul>
<li><strong>1</strong> �� <strong>N</strong> �� <strong>100000</strong></li>
<li><strong>1</strong> �� <strong>a_i</strong> �� <strong>100000</strong></li>
</ul>
<h3>Output</h3>
<p>Output the range of the minimum stretch of frost giants that could be killed in a throw. In case of multiple minimal   stretches, output the indices of that stretch that has lowest starting index.<br> If there is no such continuous stretch   possible then print -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 2 9
<strong>Output:</strong> <br>2 2<strong><br><br>Input:</strong> <br>5 <br>2 3 4 8 9
<strong>Output:</strong><br>-1<strong><br><br>Input:</strong>
10
2 4 3 5 17 4 7 5 2 15<br><strong>Output:</strong><br>7 8<br><br>
</pre>
<h3>Explanation</h3>
<p>Input #1:<br> Thor can only kill the stretch [2,2] as this is the minimum length range with strength, multiple of 3.</p>
<p>Input #2:<br> There is no stretch of frost giants that have combined strength as a multiple of 5.</p>
<p>Input #3:<br> There are many stretches of frost giants that have strength as multiple of 10. But the minimal stretch with   the least indices is from [7,8]. Minimum size stretches are [7, 8] and [8, 9]. Out of them we select [7,8].</p>