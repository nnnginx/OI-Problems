<p><em>[The original version of this problem (in Spanish) can be found at&nbsp;<a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a>]</em></p>
<p><em><br></em></p>
<p>Awari is a one-player game from the Antilles, which is played&nbsp;with boxes and stones instead of cards. A particular variant of&nbsp;Awari is played with <strong>N</strong> boxes numbered from <strong>1</strong> to <strong>N</strong>, each&nbsp;containing at the beginning of the game zero or more stones.&nbsp;The rules of this game are very simple, because there is only&nbsp;one type of valid move, consisting of choosing a box numbered <strong>i</strong>&nbsp;containing exactly <strong>i</strong> stones, and then taking those stones from&nbsp;the box in order to use them to add a single stone to every box&nbsp;numbered <strong>1</strong> through <strong>i-1</strong>; the remaining stone is then kept by the&nbsp;player. These moves are applied in succession as long as there&nbsp;exists a box <strong>i</strong> containing exactly <strong>i</strong> stones. When this is no&nbsp;longer true, the game ends. The player wins if at this stage&nbsp;every box is empty, and looses otherwise.</p>
<p>In the following figure, on the left hand side there is a&nbsp;possible initial state of a game with <strong>N = 5</strong> boxes (the circles)&nbsp;containing <strong>P<sub>1</sub> = 0</strong>, <strong>P<sub>2</sub> = 1</strong>, <strong>P<sub>3</sub> = 3</strong>, <strong>P<sub>4</sub> = 0</strong> and <strong>P<sub>5</sub> = 2</strong> stones&nbsp;(the black dots). If box number <strong>3</strong>, containing <strong>P<sub>3</sub> = 3</strong> stones,&nbsp;was chosen to make the next move, then the resulting&nbsp;configuration would be the one shown on the right hand side of&nbsp;the figure. Additionally, the player would now have one stone&nbsp;in his power.</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2012A.png" alt=""></p>
<p>Given the initial state of the boxes, you should determine if&nbsp;it is possible to win the game, that is, if there is a sequence&nbsp;of valid moves after which all the boxes are left empty.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using two lines. The first line&nbsp;contains an integer <strong>N</strong>, indicating the number of boxes (<strong>1 ��&nbsp;N&nbsp;</strong><strong>��&nbsp;500</strong>). The second line contains <strong>N</strong> integer numbers <strong>P<sub>i</sub></strong>,&nbsp;representing the number of stones in the boxes at the beginning&nbsp;of the game, from box <strong>1</strong> to box <strong>N</strong> in that order (<strong>0&nbsp;</strong><strong>��</strong><strong>&nbsp;P_i&nbsp;</strong><strong>��</strong><strong>&nbsp;500&nbsp;</strong>for <strong>i = 1, ..., N</strong>). In every test case there is at least one&nbsp;non-empty box, that is there exists <strong>i</strong> from <strong>1</strong> to <strong>N</strong> such that <strong>P<sub>i&nbsp;</sub>��&nbsp;0</strong>. The end of the input is signalled by a line containing&nbsp;the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing a&nbsp;single character. This character should be the uppercase letter&nbsp;<span style="font-family: 'courier new', courier;"><strong>'S'</strong></span> if it is possible to win the game; otherwise, it should be&nbsp;the uppercase letter <span style="font-family: 'courier new', courier;"><strong>'N'</strong></span>.</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">Awari is played with N boxes numbered from 1 to N, each</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">containing at the beginning of the game zero or more stones.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">The rules of this game are very simple, because there is only</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">one type of valid move, consisting of choosing a box numbered i</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">containing exactly i stones, and then taking those stones from</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">the box in order to use them to add a single stone to every box</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">numbered 1 through i-1; the remaining stone is then kept by the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">player. These moves are applied in succession as long as there</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">exists a box i containing exactly i stones. When this is no</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">longer true, the game ends. The player wins if at this stage</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">every box is empty, and looses otherwise.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">In the following figure, on the left hand side there is a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">possible initial state of a game with N = 5 boxes (the circles)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">containing P_1 = 0, P_2 = 1, P_3 = 3, P4 = 0 and P_5 = 2 stones</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">(the black dots). If box number 3, containing P_3 = 3 stones,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">was chosen to make the next move, then the resulting</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">configuration would be the one shown on the right hand side of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">the figure. Additionally, the player would now have one stone</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">in his power.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">[IMAGE GOES HERE]</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">Given the initial state of the boxes, you should determine if</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">it is possible to win the game, that is, if there is a sequence</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;">of valid moves after which all the boxes are left empty.</div>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5
0 1 3 0 2
4
1 1 3 0
3
1 2 3
-1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">N
S
N</span><span style="white-space: normal;">
</span></pre>