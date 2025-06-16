<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Many people know that when we think deeply about something, it even begins to show up in our dreams. Much like the story of structure of carbon attributed to Kekule. The rule of three has haunted Robert for weeks now, and has crept into his subconscious.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Robert finds himself in an N dimensional space, on a cube land of N dimensions and side 1 unit. The land is haunted by the mythological hounds Gwyllgi, three of them. Each of the 2^N vertices of the cube land is hunting ground of one of the three Gwyllgi, except those vertices that are equidistant from all three. These neutral grounds are the only places where Langdon can stand on the cube. Help Langdon find these safe grounds while he thinks of his next move to escape the cube land.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note that the distances are Manhattan distances, the smallest distance that you need to cover if movement is restricted parallel to one of the axis. Eg, distance between (0,0,0,0) and (1,0,1,1) is 3.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input consists of three lines, each line has a binary string of equal length (=N).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each string represents coordinates of a Gwyllgi in the N dimensional space, 0 meaning coordinate 0 and 1 meaning coordinate 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Eg : if the input is</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">001</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">111</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">101</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It means that in the 3D space, first Gwyllgi is at coordinate (0,0,1), second one at (1,1,1) and third one at (1,0,1)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output a single line containing number of vertices of the cube land that are safe. Since the number can be large, output the value modulo 1000000007 (10^9+7)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">111</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">001</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXPLAINATION:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Points (1,0,1) and (0,1,0) are equidistant from the three points.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CONSTRAINST:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2&lt;=N&lt;=100000</div>
<p>Many people know that when we think deeply about something, it even begins to show up in our dreams. Much like the story of structure of carbon attributed to Kekule. The rule of three has haunted Robert for weeks now, and has crept into his subconscious.</p>
<p>Robert finds himself in an <strong>N</strong> dimensional space, on a cube land of N dimensions and side 1 unit. The land is haunted by the mythological hounds Gwyllgi, three of them. Each of the 2<sup>N</sup> vertices of the cube land is hunting ground of one of the three Gwyllgi, except those vertices that are equidistant from all three. These neutral grounds are the only places where Langdon can stand on the cube. Help Langdon find these safe grounds while he thinks of his next move to escape the cube land.</p>
<p>Note that the distances are Manhattan distances, the smallest distance that you need to cover if movement is restricted parallel to one of the axis. Eg, distance between (0,0,0,0) and (1,0,1,1) is 3.</p>
<p>&nbsp;</p>
<p>INPUT:</p>
<p>Input consists of three lines, each line has a binary string of equal length (=N).</p>
<p>Each string represents coordinates of a Gwyllgi in the N dimensional space, 0 meaning coordinate 0 and 1 meaning coordinate 1.</p>
<p>Eg : if the input is</p>
<p>001</p>
<p>111</p>
<p>101</p>
<p>It means that in the 3D space, first Gwyllgi is at coordinate (0,0,1), second one at (1,1,1) and third one at (1,0,1)</p>
<p>&nbsp;</p>
<p>OUTPUT:</p>
<p>Output a single line containing number of vertices of the cube land that are safe. Since the number can be large, output the value modulo 1000000007 (10<sup>9</sup>+7)</p>
<p>&nbsp;</p>
<p>EXAMPLE INPUT:</p>
<p>111</p>
<p>001</p>
<p>100</p>
<p>&nbsp;</p>
<p>EXAMPLE OUTPUT:</p>
<p>2</p>
<p>&nbsp;</p>
<p>EXPLAINATION:</p>
<p>Points (1,0,1) and (0,1,0) are equidistant from the three points.</p>
<p>&nbsp;</p>
<p>CONSTRAINST:</p>
<p>2&lt;=N&lt;=100000</p>