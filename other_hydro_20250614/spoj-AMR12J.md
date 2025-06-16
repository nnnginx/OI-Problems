<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It was after nightfall when they had entered the Mines. They had been going for several hours with only brief halts, when Gandalf came to his first serious check. Before him stood a wide dark arch opening into three passages: all led in the same general direction, eastwards; but the left-hand passage plunged down, while the right-hand climbed up, and the middle way seemed to run on, smooth and level but very narrow. - The Fellowship of the Ring are lost in the Mines.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The Mines of Moria are a true testament of Dwarvish genius. And the Fellowship of the Ring are lost in the maze of rooms, halls and caverns. You have managed to acquire a copy of the blueprints, and if only you were part of the Fellowship, Gandalf need not have had to face the Balrog!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In this problem, we consider the Mines as consisting of rectangular rooms with their sides aligned parallel to the X (West-East) and Y (South-North) axes. Some rooms are situated within other rooms. The boundaries of any two rooms have no point in common. The rooms are numbered 0 to N-1. Your task is to determine for each room i, which room would you enter if you exit room i. If you exit into the open, output -1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, if the blueprints of the Mines looked like:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Then, you should determine that:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Room 0 exits into the open (-1)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Room 1 exits into Room 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Room 2 exits into Room 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Room 3 exits into the open (-1)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains an integer N followed by N lines. The i'th line defines the coordinates of the i'th room in the mines: x1_i, y1_i, x2_i, y2_i, where (x1_i, y1_i) are the coordinates of the southwest corner and (x2_i, y2_i) are the coordinates of the northeast corner of the i'th room.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output N lines, the i'th line containing the number of the room into which the i'th room exits. Output -1 if the i'th room exits into the open.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= N &lt;= 100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= x1_i &lt; x2_i &lt;= 1,000,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= y1_i &lt; y2_i &lt;= 1,000,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The borders of no two rooms have any point in common.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 0 10 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3 7 8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 4 5 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 10 13 15</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given in the diagram.&nbsp;</div>
<p>It was after nightfall when they had entered the Mines. They had been going for several hours with only brief halts, when Gandalf came to his first serious check. Before him stood a wide dark arch opening into three passages: all led in the same general direction, eastwards; but the left-hand passage plunged down, while the right-hand climbed up, and the middle way seemed to run on, smooth and level but very narrow. - The Fellowship of the Ring are lost in the Mines.</p>
<p>&nbsp;</p>
<p>The Mines of Moria are a true testament of Dwarvish genius. And the Fellowship of the Ring are lost in the maze of rooms, halls and caverns. You have managed to acquire a copy of the blueprints, and if only you were part of the Fellowship, Gandalf need not have had to face the Balrog!</p>
<p>&nbsp;</p>
<p>In this problem, we consider the Mines as consisting of rectangular rooms with their sides aligned parallel to the X (West-East) and Y (South-North) axes. Some rooms are situated within other rooms. The boundaries of any two rooms have no point in common. The rooms are numbered 0 to N-1. Your task is to determine for each room i, which room would you enter if you exit room i. If you exit into the open, output -1.</p>
<p>&nbsp;</p>
<p>For example, if the blueprints of the Mines looked like:</p>
<p>&nbsp;</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; -----</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;| &nbsp; &nbsp; |</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;| &nbsp; &nbsp; |</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; -----3</p>
<p>&nbsp;</p>
<p>&nbsp; &nbsp; -------------------</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp; ------- &nbsp; &nbsp; &nbsp; |</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp;| &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;|</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp;| &nbsp;[] &nbsp; | &nbsp; &nbsp; &nbsp;|</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp;| &nbsp; 2 &nbsp;| &nbsp; &nbsp; &nbsp;|</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp; -------1 &nbsp; &nbsp; |</p>
<p>&nbsp; &nbsp;| &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; |</p>
<p>&nbsp; &nbsp; ------------------0</p>
<p>&nbsp;</p>
<p>Then, you should determine that:</p>
<p>Room 0 exits into the open (-1)</p>
<p>Room 1 exits into Room 0</p>
<p>Room 2 exits into Room 1</p>
<p>Room 3 exits into the open (-1)</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains an integer N followed by N lines. The i'th line defines the coordinates of the i'th room in the mines: x1_i, y1_i, x2_i, y2_i, where (x1_i, y1_i) are the coordinates of the southwest corner and (x2_i, y2_i) are the coordinates of the northeast corner of the i'th room.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output N lines, the i'th line containing the number of the room into which the i'th room exits. Output -1 if the i'th room exits into the open.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= N &lt;= 100,000</p>
<p>0 &lt;= x1_i &lt; x2_i &lt;= 1,000,000,000</p>
<p>0 &lt;= y1_i &lt; y2_i &lt;= 1,000,000,000</p>
<p>The borders of no two rooms have any point in common.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>0 0 10 10</p>
<p>2 3 7 8</p>
<p>3 4 5 6</p>
<p>12 10 13 15</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>-1</p>
<p>0</p>
<p>1</p>
<p>-1</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>Given in the diagram.&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>