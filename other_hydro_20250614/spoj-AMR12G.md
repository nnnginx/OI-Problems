<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Strange are the ways of Men, Legolas! Here they have one of the marvels of the Northern World, and what do they say of it? Caves, they say! Caves! Holes to fly to in time of war, to store fodder in! My good Legolas, do you know that the caverns of Helm's Deep are vast and beautiful? There would be an endless pilgrimage of Dwarves, merely to gaze at them, if such things were known to be. Aye indeed, they would pay pure gold for a brief glance!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'And, Legolas, when the torches are kindled and men walk on the sandy floors under the echoing domes, ah! then, Legolas, gems and crystals and veins of precious ore glint in the polished walls; and the light glows through folded marbles, shell-like, translucent as the living hands of Queen Galadriel.' - Gimli, describing to Legolas the Glittering Caves of Aglarond.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">While these caves are by and large natural, there is one place where the Men of Rohan have chiseled into the rock to create a magnificent exhibit. You have a wall of the cave consisting of 'lighted diamonds' arranged in a N by M grid (basically, you have a light behind each diamond which can be turned on or off). Further, you have a switch corresponding to each row of this diamond-grid. When you operate a switch, it will toggle (flip) the lights corresponding to that row.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given the current configuration of the lighted diamonds. Gimli challenges Legolas to turn on as many diamonds as possible using EXACTLY K on/off operations of the switches. Since Legolas is an Elf of the Wood and doesn't care much for things that glitter, he instead asks for your help. Note that the same switch (i.e. row) can be chosen multiple times.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains the number of test cases T. Each test case contains N, M and K on the first line followed by N lines containing M characters each. The ith line denotes the state of the diamonds in the ith row, where '*' denotes a diamond which is on and '.' denotes a diamond which is off.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output T lines containing the answer for the corresponding case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Between successive test cases, there should not be any blank lines in the output.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= N,M &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= K &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 2 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">..</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">**</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 2 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">..</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">**</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first test case, row 1 can be toggled hence leaving all 4 lights to be in the ON state.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the second test case, row 1 (or row 2) can be toggled twice, hence maintaining the state of the initial configuration.&nbsp;</div>
<p>&nbsp;</p>
<p>'Strange are the ways of Men, Legolas! Here they have one of the marvels of the Northern World, and what do they say of it? Caves, they say! Caves! Holes to fly to in time of war, to store fodder in! My good Legolas, do you know that the caverns of Helm's Deep are vast and beautiful? There would be an endless pilgrimage of Dwarves, merely to gaze at them, if such things were known to be. Aye indeed, they would pay pure gold for a brief glance!</p>
<p>'And, Legolas, when the torches are kindled and men walk on the sandy floors under the echoing domes, ah! then, Legolas, gems and crystals and veins of precious ore glint in the polished walls; and the light glows through folded marbles, shell-like, translucent as the living hands of Queen Galadriel.' - Gimli, describing to Legolas the Glittering Caves of Aglarond.</p>
<p>&nbsp;</p>
<p>While these caves are by and large natural, there is one place where the Men of Rohan have chiseled into the rock to create a magnificent exhibit. You have a wall of the cave consisting of 'lighted diamonds' arranged in a N by M grid (basically, you have a light behind each diamond which can be turned on or off). Further, you have a switch corresponding to each row of this diamond-grid. When you operate a switch, it will toggle (flip) the lights corresponding to that row.</p>
<p>&nbsp;</p>
<p>You are given the current configuration of the lighted diamonds. Gimli challenges Legolas to turn on as many diamonds as possible using EXACTLY K on/off operations of the switches. Since Legolas is an Elf of the Wood and doesn't care much for things that glitter, he instead asks for your help. Note that the same switch (i.e. row) can be chosen multiple times.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T. Each test case contains N, M and K on the first line followed by N lines containing M characters each. The ith line denotes the state of the diamonds in the ith row, where '*' denotes a diamond which is on and '.' denotes a diamond which is off.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output T lines containing the answer for the corresponding case.</p>
<p>Between successive test cases, there should not be any blank lines in the output.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 100</p>
<p>1 &lt;= N,M &lt;= 50</p>
<p>1 &lt;= K &lt;= 100</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>2 2 1</p>
<p>..</p>
<p>**</p>
<p>2 2 2</p>
<p>..</p>
<p>**</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>4</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>In the first test case, row 1 can be toggled hence leaving all 4 lights to be in the ON state.</p>
<p>In the second test case, row 1 (or row 2) can be toggled twice, hence maintaining the state of the initial configuration.&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>