<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Hoo, ho! Good morning, Merry and Pippin!' he boomed, when he saw them. 'You sleep long. I have been many a hundred strides already today. Now we will have a drink, and go to Entmoot.'</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Where is Entmoot?' Pippin ventured to ask.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Hoo, eh? Entmoot?' said Treebeard, turning round. 'It is not a place, it is a gathering of Ents - which does not often happen nowadays. But I have managed to make a fair number promise to come.'</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Indeed, Entmoot cannot be thought of as any particular place, since where it occurs changes from time to time. The choice of the location however, follows a basic principle: Although the Ents (walking and talking Trees - "shepherds of Fangorn Forest") are by and large not hasty, when it comes to gathering for Entmoot, they would like to choose a location that ensures all the Ents can reach as soon as possible.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note however, that the speed they can travel varies from Ent to Ent. Also, although Fangorn Forest has dense overgrowth, with regard to the Ents, the forest poses no obstacles.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given the locations of N Ents who have agreed to join in for Entmoot, as well as their speeds. You need to find out where Entmoot will occur. Formally, given the (x_i,y_i) along with speed s_i for each Ent, find the point (X, Y) such that the maximum time taken by any of the Ents to reach (X, Y) is minimized. Output the earliest time when all the Ents can meet.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains T, the number of test cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line of each test case contains N, the number of Ents.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The next N lines contain three space-separated integers each. The ith of these lines contains : x_i, y_i, s_i.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output one line per test case, containing the earliest time when the Ents can meet. Relative and absolute error of 10^-4 are acceptable.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 &lt;= N &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1,000,000 &lt;= x_i, y_i &lt;= 1,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= s_i &lt;= 1,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4 0 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-3 -4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 10 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 20 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 40 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 100 15</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 -100 15</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">8 0 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">10000 0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5000 8661 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1.000000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">7.500000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">6.666667</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5773.751357</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first test case, all the ents can meet at origin in 1 unit of time.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the second test case, the first and the third ent reach (25,0) after 7.5 units of ime, whereas the second ent reaches there after 2.5 units of time and waits for the remaining ents to arrive.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the third test case, all the ents can meet at origin in 100/15 units of time.</div>
<p>&nbsp;</p>
<p>Hoo, ho! Good morning, Merry and Pippin!' he boomed, when he saw them. 'You sleep long. I have been many a hundred strides already today. Now we will have a drink, and go to Entmoot.'</p>
<p>'Where is Entmoot?' Pippin ventured to ask.</p>
<p>'Hoo, eh? Entmoot?' said Treebeard, turning round. 'It is not a place, it is a gathering of Ents - which does not often happen nowadays. But I have managed to make a fair number promise to come.'</p>
<p>&nbsp;</p>
<p>Indeed, Entmoot cannot be thought of as any particular place, since where it occurs changes from time to time. The choice of the location however, follows a basic principle: Although the Ents (walking and talking Trees - "shepherds of Fangorn Forest") are by and large not hasty, when it comes to gathering for Entmoot, they would like to choose a location that ensures all the Ents can reach as soon as possible.</p>
<p>&nbsp;</p>
<p>Note however, that the speed they can travel varies from Ent to Ent. Also, although Fangorn Forest has dense overgrowth, with regard to the Ents, the forest poses no obstacles.</p>
<p>&nbsp;</p>
<p>You are given the locations of N Ents who have agreed to join in for Entmoot, as well as their speeds. You need to find out where Entmoot will occur. Formally, given the (x_i,y_i) along with speed s_i for each Ent, find the point (X, Y) such that the maximum time taken by any of the Ents to reach (X, Y) is minimized. Output the earliest time when all the Ents can meet.&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains T, the number of test cases.</p>
<p>The first line of each test case contains N, the number of Ents.</p>
<p>The next N lines contain three space-separated integers each. The ith of these lines contains : x_i, y_i, s_i.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output one line per test case, containing the earliest time when the Ents can meet. Relative and absolute error of 10^-4 are acceptable.&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 10</p>
<p>2 &lt;= N &lt;= 50</p>
<p>-1,000,000 &lt;= x_i, y_i &lt;= 1,000,000</p>
<p>1 &lt;= s_i &lt;= 1,000,000</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>3</p>
<p>0 3 3</p>
<p>4 0 4</p>
<p>-3 -4 5</p>
<p>3</p>
<p>0 10 2</p>
<p>0 20 2</p>
<p>0 40 2</p>
<p>3</p>
<p>0 100 15</p>
<p>0 -100 15</p>
<p>8 0 7</p>
<p>3</p>
<p>0 0 1</p>
<p>10000 0 1</p>
<p>5000 8661 1</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>1.000000</p>
<p>7.500000</p>
<p>6.666667</p>
<p>5773.751357</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>In the first test case, all the ents can meet at origin in 1 unit of time.&nbsp;</p>
<p>In the second test case, the first and the third ent reach (25,0) after 7.5 units of ime, whereas the second ent reaches there after 2.5 units of time and waits for the remaining ents to arrive.&nbsp;</p>
<p>In the third test case, all the ents can meet at origin in 100/15 units of time.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>