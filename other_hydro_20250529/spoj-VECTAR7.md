<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Changu and Mangu were playing volleyball, when they were handed a very easy question about the game.You can help them solve it.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">In volleyball 2 teams play with initial score 0 and each team gets points which increases their</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">scores by 1.&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">The game ends when:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">One of the teams gets 25 points and another team has &lt; 24 points ( strictly less than 24).</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">If the score ties at 24:24, the teams continue to play until the absolute difference between the scores is 2.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Given the final score of a game ( A B ) i.e., the first team has scored A points and the second has scored B points,</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">You have to find the number of different sequences of getting points by teams that leads to this final score?</span></div>
<p><span style="font-size: small;">Changu and Mangu were playing volleyball when they were handed a very easy question about the game. You can help them solve it.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">In volleyball 2 teams play with initial score 0 and each team gets points which increases their&nbsp;scores by 1.&nbsp;</span></p>
<p><span style="font-size: small;">The game ends when:</span></p>
<p><span style="font-size: small;">One of the teams gets 25 points and another team has &lt; 24 points ( strictly less than 24).</span></p>
<p><span style="font-size: small;">If the score ties at 24:24, the teams continue to play until the absolute difference between the scores is 2.</span></p>
<p><span style="font-size: small;">Given the final score of a game ( A B ) i.e., the first team has scored A points and the second has scored B points,</span></p>
<p><span style="font-size: small;">You have to find the number of different sequences of getting points by teams that leads to this final score?</span></p>
<p>&nbsp;</p>
<h3><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;">The first line contains the number of test cases T. The next T lines contain two integers A and B.</span></p>
<h3><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;"><span style="color: #39424e; line-height: 24px;">Output the number of different sequences of getting points by the teams that leads to the final score A : B.&nbsp;</span><em>Final&nbsp;</em><span style="color: #39424e; line-height: 24px;">means that the game should be over after this score is reached. If the number is larger than 10</span><span style="border: 0px; font-stretch: inherit; line-height: 0; margin: 0px; outline: 0px; padding: 0px; vertical-align: baseline; position: relative; top: -0.5em; word-wrap: break-word; word-break: break-word; color: #39424e;">9</span><span style="color: #39424e; line-height: 24px;">+7, output number modulo 10</span><span style="border: 0px; font-stretch: inherit; line-height: 0; margin: 0px; outline: 0px; padding: 0px; vertical-align: baseline; position: relative; top: -0.5em; word-wrap: break-word; word-break: break-word; color: #39424e;">9</span><span style="color: #39424e; line-height: 24px;">&nbsp;+ 7. Print 0</span><span style="color: #39424e; line-height: 24px;">&nbsp;if no such volleyball game ends with the given score.</span></span></p>
<h3><span style="font-size: small;">Example</span></h3>
<p><strong><span style="font-size: small;">Input:</span></strong></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">3 25</span></p>
<p><span style="font-size: small;">24 17</span></p>
<p><span style="font-size: small;">&nbsp;</span><span style="font-size: small; font-weight: bold;">Output:</span></p>
<p><span style="font-size: small;">2925</span><span style="white-space: normal;">&nbsp;</span></p>
<p><span style="font-size: small;">0</span></p>
<p><span style="font-size: small;"><strong>Constraints:</strong></span></p>
<p><span style="font-size: small;">T&lt;=15</span></p>
<p><span style="font-size: small;"><span style="color: #39424e; line-height: 24px;">0 ¡Ü A , B ¡Ü 10</span><span style="border: 0px; font-stretch: inherit; line-height: 0; margin: 0px; outline: 0px; padding: 0px; vertical-align: baseline; position: relative; top: -0.5em; word-wrap: break-word; word-break: break-word; color: #39424e;">9</span></span></p>