<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<p><span style="font-style: italic;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The domino effect is a phenomenon that occurs when in a line of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">domino pieces, each standing on its smallest face, the first</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">piece from one of the line's ends falls in the direction of the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">next piece. In turn, this second piece falls over the third one</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">in the line, and so on until the other end of the line is</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">reached, at which point every piece has fallen. Note that in</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">order to produce this effect, the distance between consecutive</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">pieces in the line must be lower or equal to their height.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Emma has very recently found out about the domino effect, and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">she was immediately amazed by it. She spent all morning forming</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">a line with the N domino pieces that her brother Ezequiel gave</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">her, but just before she was going to make the first piece</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">fall, her grandma came to her home and took her to play in the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">park. Ezequiel knows Emma has not taken into account the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">distance between consecutive pieces when she formed her domino</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">line, and doesn't want to see her frustrated if all the pieces</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">do not fall after she pushes the first one. Thus, Ezequiel</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">wants to move some pieces from inside the line so that the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">distance between consecutive pieces is always lower or equal to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">their height H. Because he doesn't want Emma to find out that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">he has moved some of the pieces, que will leave the first and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">last pieces where they are, and he would also like to move as</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">few pieces as possible from inside the line. What is the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">minimum number of pieces he must move?</div>
<p>The <em>domino effect</em> is a phenomenon that occurs when in a line of&nbsp;domino pieces, each standing on its smallest face, the first&nbsp;piece from one of the line's ends falls in the direction of the&nbsp;next piece. In turn, this second piece falls over the third one&nbsp;in the line, and so on until the other end of the line is&nbsp;reached, at which point every piece has fallen. Note that in&nbsp;order to produce this effect, the distance between consecutive&nbsp;pieces in the line must be lower or equal to their height.</p>
<p>Emma has very recently found out about the domino effect, and&nbsp;she was immediately amazed by it. She spent all morning forming&nbsp;a line with the <strong>N</strong> domino pieces that her brother Ezequiel gave&nbsp;her, but just before she was going to make the first piece&nbsp;fall, her grandma came to her home and took her to play in the&nbsp;park. Ezequiel knows Emma has not taken into account the&nbsp;distance between consecutive pieces when she formed her domino&nbsp;line, and doesn't want to see her frustrated if all the pieces&nbsp;do not fall after she pushes the first one. Thus, Ezequiel&nbsp;wants to move some pieces from inside the line so that the&nbsp;distance between consecutive pieces is always lower or equal to&nbsp;their height <strong>H</strong>. Because he doesn't want Emma to find out that&nbsp;he has moved some of the pieces, he will leave the first and&nbsp;last pieces where they are, and he would also like to move as few pieces as possible from inside the line. What is the&nbsp;minimum number of pieces he must move?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using two lines. The first line&nbsp;contains two integer numbers <strong>N</strong> and <strong>H</strong>, indicating respectively&nbsp;the number of pieces in the line (<strong>3 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;1000</strong>) and their&nbsp;height (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;H&nbsp;</strong><strong>��</strong><strong>&nbsp;50</strong>). The second line contains <strong>N-1</strong> integers <strong>D<sub>i</sub></strong>, representing the distances between pairs of consecutive&nbsp;domino pieces, in the order given by the line (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;D<sub>i</sub>&nbsp;<strong>��&nbsp;</strong>100</strong>&nbsp;for <strong>i = 1, 2, ..., N-1</strong>). The end of the input is signalled by a&nbsp;line containing two times the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a line containing a single&nbsp;integer number, representing the minimum number of pieces that&nbsp;must be moved in order to have the distance between consecutive pieces always lower or equal to <strong>H</strong>. Note that the first and last pieces cannot be moved, and that the relative order between the the pieces cannot be changed. If it is impossible to achieve the desired result, print the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">8 3
2 4 4 1 4 3 2
10 2
1 2 2 2 2 2 2 2 3
5 2
2 2 2 2
5 3
1 6 2 4
-1 -1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
8
0
-1</span><span style="white-space: normal;">
</span></pre>