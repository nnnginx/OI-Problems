<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You have an N * M chessboard on which some squares are blocked out. In how many ways can you place one or more queens on the board such that no two queens attack each other? Two queens attack each other if one can reach the other by moving horizontally, vertically or diagonally without passing over any blocked square. At most one queen can be placed on a square. A queen cannot be placed on a blocked square.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow. Each test case contains integers N and M on the first line. The following N lines contain M characters each representing the board. A '#' represents a blocked square and a '.' represents an unblocked square.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines containing the required answer for each test case. As the answers can be really large, output them modulo 1000000007.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= N &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= M &lt;= 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">.#.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">.#.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">.#..</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">....</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">#</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">17</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">18</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">14</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0</div>
<p>&nbsp;</p>
<p>You have an N * M chessboard on which some squares are blocked out. In how many ways can you place one or more queens on the board such that no two queens attack each other? Two queens attack each other if one can reach the other by moving horizontally, vertically or diagonally without passing over any blocked square. At most one queen can be placed on a square. A queen cannot be placed on a blocked square.</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. T test cases follow. Each test case contains integers N and M on the first line. The following N lines contain M characters each representing the board. A '#' represents a blocked square and a '.' represents an unblocked square.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines containing the required answer for each test case. As the answers can be really large, output them modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 100</p>
<p>1 &lt;= N &lt;= 50</p>
<p>1 &lt;= M &lt;= 5</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>3 3</p>
<p>...</p>
<p>...</p>
<p>...</p>
<p>3 3</p>
<p>.#.</p>
<p>.#.</p>
<p>...</p>
<p>2 4</p>
<p>.#..</p>
<p>....</p>
<p>1 1</p>
<p>#</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>17</p>
<p>18</p>
<p>14</p>
<p>0</p>
<p>&nbsp;</p>