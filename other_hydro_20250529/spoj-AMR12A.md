<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'Hush!' said Frodo. 'I think I hear hoofs again.'</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">They stopped suddenly and stood as silent as tree-shadows, listening. There was a sound of hoofs in the lane, some way behind, but coming slow and clear down the wind. Quickly and quietly they slipped off the path, and ran into the deeper shade under the oak-trees.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The hoofs drew nearer. They had no time to find any hiding-place better than the general darkness under the trees.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- Frodo, Sam and Pippin, when they encounter a Black Rider.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Indeed, the Black Riders are in the Shire, and they are looking for the One Ring. There are N hobbits out in their fields, but when they hear the Riders approaching, or feel the fear cast by their presence, they immediately wish to run and hide in M holes located nearby.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now, each hole has space for just 1 hobbit; however, once a hobbit reaches a hole, he is able to make room for one more hobbit by digging away at the earth. The time required to make enough space for a second hobbit is C units. Also, each hole CANNOT hold more than 2 hobbits, even after digging. Also note that a hobbit can begin making space for the next hobbit only after he reaches the hole.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given the time required to travel from each hobbit's current location to each hole. Find the minimum amount of time it will take before at least K of the hobbits are hiding safely.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains T, the number of test cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line of each test case contains 4 integers - N (no of hobbits), M (no of holes), K (minimum number of hobbits to hide) and C (time taken to expand a hole).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The next N lines contain M integers each, denoting the time taken for each hobbit to each hole.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output one line per test case which contains the minimum time.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= N, M &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= K &lt;= min(N, 2 * M)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt; C &lt; 10,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt; Time taken by the hobbits to the holes &lt; 10,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Time Limit: 2s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Memory Limit: 64MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 3 2 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">9 11 13</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 10 14</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 15 12</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4 3 3 8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 10 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 10 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">100 100 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 10 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the first test case, there are 3 hobbits and 3 holes, and we need to get atleast 2 of them to safety. We can send the first hobbit to the first hole, and the second hobbit to the second hole, thereby taking 10 time units.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the second test case, we can make hobbit #1 reach hole 1 at time 1, hobbit #2 reach hole 1 at time 9 (by when hobbit #1 would have finished digging the hole), and hobbit #3 reach hole 3 at time 6.</div>
<p>'Hush!' said Frodo. 'I think I hear hoofs again.'</p>
<p>They stopped suddenly and stood as silent as tree-shadows, listening. There was a sound of hoofs in the lane, some way behind, but coming slow and clear down the wind. Quickly and quietly they slipped off the path, and ran into the deeper shade under the oak-trees.</p>
<p>The hoofs drew nearer. They had no time to find any hiding-place better than the general darkness under the trees.&nbsp;</p>
<p>- Frodo, Sam and Pippin, when they encounter a Black Rider.</p>
<p>&nbsp;</p>
<p>Indeed, the Black Riders are in the Shire, and they are looking for the One Ring. There are N hobbits out in their fields, but when they hear the Riders approaching, or feel the fear cast by their presence, they immediately wish to run and hide in M holes located nearby.</p>
<p>&nbsp;</p>
<p>Now, each hole has space for just 1 hobbit; however, once a hobbit reaches a hole, he is able to make room for one more hobbit by digging away at the earth. The time required to make enough space for a second hobbit is C units. Also, each hole CANNOT hold more than 2 hobbits, even after digging. Also note that a hobbit can begin making space for the next hobbit only after he reaches the hole.</p>
<p>&nbsp;</p>
<p>You are given the time required to travel from each hobbit's current location to each hole. Find the minimum amount of time it will take before at least K of the hobbits are hiding safely.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>&nbsp;</p>
<p>The first line contains T, the number of test cases.</p>
<p>The first line of each test case contains 4 integers - N (no of hobbits), M (no of holes), K (minimum number of hobbits to hide) and C (time taken to expand a hole).</p>
<p>The next N lines contain M integers each, denoting the time taken for each hobbit to each hole.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>&nbsp;</p>
<p>Output one line per test case which contains the minimum time.&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 6</p>
<p>1 &lt;= N, M &lt;= 100</p>
<p>1 &lt;= K &lt;= min(N, 2 * M)</p>
<p>0 &lt; C &lt; 10,000,000</p>
<p>0 &lt; Time taken by the hobbits to the holes &lt; 10,000,000</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3 3 2 10</p>
<p>9 11 13</p>
<p>2 10 14</p>
<p>12 15 12</p>
<p>4 3 3 8</p>
<p>1 10 100</p>
<p>1 10 100</p>
<p>100 100 6</p>
<p>12 10 10</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>10</p>
<p>9</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>For the first test case, there are 3 hobbits and 3 holes, and we need to get atleast 2 of them to safety. We can send the first hobbit to the first hole, and the second hobbit to the second hole, thereby taking 10 time units.</p>
<p>For the second test case, we can make hobbit #1 reach hole 1 at time 1, hobbit #2 reach hole 1 at time 9 (by when hobbit #1 would have finished digging the hole), and hobbit #3 reach hole 3 at time 6.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>