<p>&nbsp;</p>
<p>There is a faceoff between Spiderman &amp; Sandman.&nbsp;</p>
<p>There are two glass buildings each of height H. Each building has H equal sized windows on the outside covering entire space from bottom to top. Some windows are open and spiderman cannot land on these window.</p>
<p>In one step, Spiderman can:</p>
<p>1) Rise up to just above window of the same building he is on.</p>
<p>2) Slide down to just below window of the same building he is on.</p>
<p>3) Use his web to jump to Kth window above from current height on the other building.</p>
<p>&nbsp;</p>
<p>Sandman on the other rises steadily a rate of 1 per step.</p>
<p>For the purpose of this problem, assume Spiderman and Sandman take turns ie: Spiderman takes one step, then Sandman takes one step.</p>
<p>Your goal is to assist Spiderman to always remain above or at same height as Sandman at the end of Sandman's turn. Spiderman gets the first turn and both start at height 0 (ie: Sandman is on the ground and Spiderman is on the window of lowermost floor of left building. It is guarenteed that window of lowermost floor of left building is not open.</p>
<p>Note : If Spiderman gets to area with height &gt;= H assume he has got out.</p>
<p>&nbsp;</p>
<p>You are Spiderman's best friend, your duty is to guide Spiderman to escape from Sandman if possible in shortest number of steps to get out.</p>
<p>&nbsp;</p>
<p><strong>Input</strong></p>
<p>First line contains integer T.&nbsp;</p>
<p>T Testcases follow. Each testcase contains 3 lines.&nbsp;</p>
<p>First line of input contains two space seperated integers H &amp; K</p>
<p>Next two lines contain description of two buildings.</p>
<p>2nd line represents the left building - a string of length H. The ith character represents the state of window between (i-1) and i heights : character '-' represents closed window(safe to land on) , character 'X' represents open window.&nbsp;</p>
<p>Similarly 3rd line represents the right building.</p>
<p>&nbsp;</p>
<p><strong>Output</strong></p>
<p>For every testcase output single integer x where x is the number of steps taken to get out of building. Output "NO" if Spiderman cannot escape the area and has to fight in the enclosure.</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong></p>
<p>1&lt;=T&lt;=10</p>
<p>1 &lt;= H,K &lt;= 10^5</p>
<p>&nbsp;</p>
<p><strong>Example</strong></p>
<p>Input:&nbsp;</p>
<p>2</p>
<p>7 3</p>
<p>---X--X</p>
<p>-X--XX-</p>
<p>6 2</p>
<p>--X-X-</p>
<p>X--XX-</p>
<p>&nbsp;</p>
<p>Output:&nbsp;</p>
<p>4</p>
<p>NO</p>
<p>&nbsp;</p>
<p>EXPLANATION</p>
<p>In first case Spiderman jumps to right building, goes one height down, jumps to left building and jumps to right buidling (he got to the top).</p>
<p>In second case, no matter how he moves, Spiderman cannot escape above the buildings.</p>
<p>&nbsp;</p>