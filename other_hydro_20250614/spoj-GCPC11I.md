<p><img src="../../../content/ak15:weavers.jpg" alt="example image" hspace="10" vspace="10" width="25%" align="right"></p>
<p>Willy the Weaver is in desperate hope to get married to the most beautiful and delightful female weaver Wilmar. Of course, Willy is not the only weaver interested in Wilmar.</p>
<p>In order to impress the females, weavers build elaborately woven nests using leaf fibers. Tomorrow is the big day on which Wilmar will inspect all nests. There is a heavy storm at the moment, and no weaver can leave his nest within the hours before sunrise. However, the storm will produce many piles of leaf fibers, so that all weavers will have a chance to improve their nests. Therefore, Willy is curious if he can succeed weaving the most impressive nest, so that Wilmar will finally decide on getting married to him. Since size matters, Willy tries to figure out how large his nest and the ones of his rivals may become.</p>
<p>For this purpose, Willy takes into consideration all known places offering leaf fibers suitable for nest construction. Since weavers do not like to leave their known territory, many of these places can be accessed by a subset of all weavers only, and some might even not be reachable by any weaver.</p>
<p>To reduce complexity, Willy does not want to set up a flight plan. This implies that he does not consider any particular strategy of his rivals nor does he make any assumptions on how many fibers they can carry at a time or how quick and when they fly. It is therefore possible that a weaver succeeds in picking up all fibers in his territory. Finally, Willy assumes that all weavers are as integer as he is: they do not steal fibers from nests of their rivals.</p>
<p>Is there any chance that no weaver will have a larger nest (number of fibers) than Willy after all leaf fibers have been picked up?</p>
<h3>Input</h3>
<p>The first line contains the number of testcases <em>T</em> (<em>1 �� T �� 100</em>). Each test case starts with a line containing two integers. The first integer <em>W</em> (<em>1 �� W �� 100</em>) is the number of weavers (including Willy); the second one <em>P</em> (<em>1 �� P �� 400</em>) is the number of places with leaf fibers.</p>
<p>Next come <em>W</em> lines describing the nest of each weaver with four integers <em>x</em>, <em>y</em>, <em>f</em>, and <em>r</em> (<em>0 �� x, y, r �� 10000</em>, <em>1 �� f �� 10000</em>): <em>x</em> and <em>y</em> define the position of the nest, <em>f</em> is the size of the nest in number of fibers, and <em>r</em> is the radius of the territory in which the owner of the nest will search for additional fibers. The first of these <em>W</em> lines describes Willy's nest.</p>
<p>Thereafter follow <em>P</em> lines defining the places with available leaf fibers with three integers <em>x</em>, <em>y</em>, and <em>f</em> (<em>0 �� x, y �� 10000</em>, <em>1 �� f �� 10000</em>): <em>x</em> and <em>y</em> define the position of the place, and <em>f</em> is the number of available leaf fibers.</p>
<h3>Output</h3>
<p>For each test case print one single line containing the string <strong>Suiting Success</strong>, if Willy has a chance to marry Wilmar after all fibers have been picked up (a tie in nest size is sufficient); else print <strong>Lonesome Willy</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 2
0 0 1 10
10 0 1 10
20 0 1 10
5 0 2
15 0 4
3 2
0 0 1 10
10 0 1 10
20 0 1 10
5 0 2
15 0 5

<strong>Output:</strong>
Suiting Success
Lonesome Willy
</pre>