<p><em><strong>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</strong></em></p>
<p>In the kingdom of Nlogonia there is a lake known as the "<em>Big O</em>" because of its perfectly round shape. On the side of this lake there are <strong>N</strong> houses, each of them a distance of one nlogonic unit apart from its neighbors. The houses are numbered from <strong>1</strong> to <strong>N</strong> in clockwise order, as can be seen in the following figure for <strong>N = 8</strong>.</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2013D.png" alt="TAP2013D"></p>
<p>In this way, if <strong>i &lt; j</strong> the distance in clockwise order from house <strong>i</strong> to house <strong>j</strong> is <strong>j-i</strong>, whereas the corresponding distance in counterclockwise order is <strong>N - j + i</strong>. Note that the distance from a house to itself is <strong>N</strong> in both directions.</p>
<p>It is well known that the people of Nlogonia are avid football fans, so when a family moves to a house on the side of the lake it is very important for them to know who are their closest neighbors that follow the same team as they do. This is not always easy, since there may be many houses around the lake, many different football teams in Nlogonia, and a lot of moving around. Given a sequence of <strong>M</strong> movings, people who live on the shore of the lake want to welcome each new family arriving by telling them the distance from their new home to the closest houses that follow the same team as they do, both in clockwise and counterclockwise order. Note that if there is no other house on the shore of the lake whose family follows the same team as the newly arrived, said distance shall be <strong>N</strong> in both directions, as the closest house would in fact be the same house involved in the moving. Do you want to take part in the welcoming committee?</p>
<p>In Nlogonia there are <strong>F</strong> football teams, identified by different integer numbers from <strong>0</strong> to <strong>F-1</strong>. Because we don't want you to waste any time going from door to door asking which team is followed in each house, we will assume that initially the family living in house number <strong>i</strong> is a fan of team number <strong>e<sub>i</sub></strong>, being this number generated in pseudo-random fashion by the recursive formula</p>
<p style="text-align: center;"><strong>e<sub>1</sub> = A &nbsp; &nbsp;&nbsp;</strong>and &nbsp; &nbsp;&nbsp;<strong>e<sub>i</sub> = (B ��&nbsp;e<sub>i-1</sub>&nbsp;+ C) mod F &nbsp; &nbsp;&nbsp;</strong>for &nbsp; &nbsp;&nbsp;<strong>i = 2, 3, ..., N</strong></p>
<p>where <strong>A</strong>, <strong>B</strong> and <strong>C</strong> are constants and the expression <strong>x mod y</strong> represents the remainder of the integer division of <strong>x</strong> by <strong>y</strong>.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integer numbers <strong>N</strong> and <strong>F</strong>, respectively indicating the number of houses around the lake and the number of football teams in Nlogonia (<strong>3 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong> and <strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;F&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>6</sup></strong>). The second line contains three integer numbers <strong>A</strong>, <strong>B</strong> and <strong>C</strong>, which determine which team is followed by the families initially living around the lake as is described in the problem statement (<strong>0&nbsp;</strong><strong>��</strong><strong>&nbsp;A, B, C &lt; F</strong>).</p>
<p>The third line contains a single integer number <strong>M</strong>, representing the number of movings that will be happening (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;M&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong>). Each of the following <strong>M</strong> lines describes a moving using two integer numbers <strong>I</strong> and <strong>E</strong>, meaning that a family following team <strong>E</strong> is moving to house number <strong>I</strong> (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;I&nbsp;</strong><strong>��</strong><strong>&nbsp;N</strong> and <strong>0&nbsp;</strong><strong>��</strong><strong>&nbsp;E &lt; F</strong>). The movings appear in the order that they occur, and should be taken into account by the committee for further welcomings.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print <strong>M</strong> lines, the <strong>i</strong>-th of them indicating the result of the <strong>i</strong>-th moving described in the input. Each line should contain two integer numbers <strong>d<sub>ccw</sub></strong> and <strong>d<sub>cw</sub></strong>, representing the distances in nlogonic units from the house involved in the moving to the first house whose family follows the same team, in counterclockwise and clockwise order respectively.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5 10
1 1 1
6
1 1
2 2
3 1
4 2
5 1
3 1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">5 5
5 5
2 3
2 3
2 1
2 2</span><span style="white-space: normal;">
</span></pre>