<p>&nbsp;</p>
<p>The wizards and witches of Hogwarts School of Witchcraft found Prof. Binn's History of Magic lesson to be no less boring than you found your own history classes. &nbsp;Recently Binns has been droning on about Goblin wars, and which goblin civilization fought which group of centaurs where etc etc. &nbsp;The students of Hogwarts decided to use the new-fangled computer to figure out the outcome of all these wars instead of memorizing the results for their upcoming exams. &nbsp;Can you help them?</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">civilization fought which group of centaurs where etc etc. &nbsp;The students of Hogwarts decided to use the new-fangled computer to figure out the outcome of all these wars instead of memorizing the results for their upcoming exams. &nbsp;Can you help them?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The magical world looks like a 2-D R*C grid. Initially there are many civilizations, each civilization occupying exactly one cell. A civilization is denoted by a lowercase letter in the grid. There are also certain cells that are uninhabitable (swamps, mountains, sinkholes etc.) - these cells are denoted by a '#' in the grid. All the other cells - to which the civilizations can move &nbsp;- are represented by a '.' in the grid.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A cell is said to be adjacent to another cell if they share the same edge - in other words, for a cell (x,y), cells (x-1, y), (x, y-1), (x+1, y), (x, y+1) are adjacent, provided they are within the boundaries of the grid. &nbsp; Every year each civilization will expand to all unoccupied adjacent cells. If it is already inhabited by some other civilization, it just leaves the cell alone. It is possible that two or more civilizations may move into an unoccupied cell at the same time - this will lead to a battle between the civilizations and the cell will be marked with a '*'. Note that the civilizations fighting in a particular cell do not try to expand from that cell, but will continue to expand from other cells, if possible.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given the initial grid, output the final state of the grid after no further expansion by any civilization is possible.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains T, the number of cases. This is followed by T test case blocks.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each test case contains two integers, R, C.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">This is followed by R lines containing a string of length C. The j-th letter in the i-th row describes the state of the cell in year 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each cell is either a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1. '.' which represents an unoccupied cell</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2. '#' which represents a cell that cannot be occupied</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3. A civilization represented by a lowercase letter ('a' - 'z')</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For each test case, print the final grid after no expansion is possible. Apart from the notations used in the input, use '*' to denote that a battle is being waged in that particular cell.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Print a blank line at the end of each case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= R, C &lt;= 500</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: &nbsp;3 s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 64 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a...b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a..b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#c#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a.b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#d#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#c#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a.b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">.....</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">.#.#.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a...b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">aa*bb</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">aabb</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">####</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#c#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a*b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#d#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#c#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">acb</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a*b</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">aa*bb</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a#.#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">aa*bb</div>
<p>The magical world looks like a 2-D R*C grid. Initially there are many civilizations, each civilization occupying exactly one cell. A civilization is denoted by a lowercase letter in the grid. There are also certain cells that are uninhabitable (swamps, mountains, sinkholes etc.) - these cells are denoted by a '#' in the grid. All the other cells - to which the civilizations can move &nbsp;- are represented by a '.' in the grid.</p>
<p>&nbsp;</p>
<p>A cell is said to be adjacent to another cell if they share the same edge - in other words, for a cell (x,y), cells (x-1, y), (x, y-1), (x+1, y), (x, y+1) are adjacent, provided they are within the boundaries of the grid. &nbsp; Every year each civilization will expand to all unoccupied adjacent cells. If it is already inhabited by some other civilization, it just leaves the cell alone. It is possible that two or more civilizations may move into an unoccupied cell at the same time - this will lead to a battle between the civilizations and the cell will be marked with a '*'. Note that the civilizations fighting in a particular cell do not try to expand from that cell, but will continue to expand from other cells, if possible.</p>
<p>Given the initial grid, output the final state of the grid after no further expansion by any civilization is possible.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains T, the number of cases. This is followed by T test case blocks.</p>
<p>Each test case contains two integers, R, C.</p>
<p>This is followed by R lines containing a string of length C. The j-th letter in the i-th row describes the state of the cell in year 0.</p>
<p>Each cell is either a</p>
<p>1. '.' which represents an unoccupied cell</p>
<p>2. '#' which represents a cell that cannot be occupied</p>
<p>3. A civilization represented by a lowercase letter ('a' - 'z')</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each test case, print the final grid after no expansion is possible. Apart from the notations used in the input, use '*' to denote that a battle is being waged in that particular cell.&nbsp;</p>
<p>Print a blank line at the end of each case.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= R, C &lt;= 500</p>
<p>1 &lt;= T &lt;= 5</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>5</p>
<p>3 5</p>
<p>#####</p>
<p>a...b</p>
<p>#####</p>
<p>3 4</p>
<p>####</p>
<p>a..b</p>
<p>####</p>
<p>3 3</p>
<p>#c#</p>
<p>a.b</p>
<p>#d#</p>
<p>3 3</p>
<p>#c#</p>
<p>...</p>
<p>a.b</p>
<p>3 5</p>
<p>.....</p>
<p>.#.#.</p>
<p>a...b</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>#####</p>
<p>aa*bb</p>
<p>#####</p>
<p>&nbsp;</p>
<p>####</p>
<p>aabb</p>
<p>####</p>
<p>&nbsp;</p>
<p>#c#</p>
<p>a*b</p>
<p>#d#</p>
<p>&nbsp;</p>
<p>#c#</p>
<p>acb</p>
<p>a*b</p>
<p>&nbsp;</p>
<p>aa*bb</p>
<p>a#.#b</p>
<p>aa*bb</p>
<p>&nbsp;</p>
<p>&nbsp;</p>