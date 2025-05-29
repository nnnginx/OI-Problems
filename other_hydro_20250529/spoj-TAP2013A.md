<p><em><strong>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</strong></em></p>
<p>On the side of the road, there are palm trees, there's a bar, there's shadow, there's something more. In this problem, we are particularly interested in the palm trees.</p>
<p>Ana, Adan, Alan and Amanda organized a trip: while Ana and Adan where dealing with petty things like checking the car, preparing the luggage and finding a place to stay, Alan and Amanda dedicated themselves to the most important part: studying the views of palm trees to which they would have access to while on the road.</p>
<p>The road they are now driving on is completely straight, and in this problem we will represent it by the <strong>Y = 0</strong> line of the <strong>XY</strong> plane. On the side of the road with coordinates <strong>Y &gt; 0</strong> there are palm trees, which we will represent by different points of the <strong>XY</strong> plane with positive <strong>Y</strong> coordinate. Alan and Amanda have noticed that from each point on the road certain palm trees are visible, and in general these vary along the road. A palm tree is said to be visible from a point on the road if and only if the segment that joins both points does not go through any other palm tree.</p>
<p>In the following figure the unfilled circles represent palm trees in the first sample input, whereas the filled ones represent some possible points on the road.</p>
<p style="text-align: center;"><img src="../../content/fidels:TAP2013A.png" alt="TAP2013A"></p>
<p>From point <strong>p</strong> the palm trees that are visible are <strong>a</strong>, <strong>b</strong> and <strong>d</strong>, since palm tree <strong>c</strong> is hidden behind palm tree <strong>a</strong>. From point <strong>q</strong> the visible palm trees are <strong>a</strong>, <strong>c</strong> and <strong>d</strong>, since palm tree <strong>b</strong> is now hidden behind palm tree <strong>a</strong>. From point <strong>r</strong> all the palm trees are visible, and from point <strong>s</strong> only palm trees <strong>a</strong> and <strong>d</strong> are visible, since palm trees <strong>b</strong> and <strong>c</strong> are hidden behind palm tree <strong>d</strong>.</p>
<p>While Ana and Adan take turns to drive the car, Alan and Amanda discuss the benefits of knowing how many visible quantities of palm trees there are. Given a set of palm trees, an integer number <strong>m</strong> is a visible quantity of palm trees if and only if there exists at least one point on the road (i.e. a point with coordinate <strong>Y = 0</strong>) from which exactly <strong>m</strong> palm trees are visible.</p>
<p>In the example illustrated above, <strong>2</strong>, <strong>3</strong> and <strong>4</strong> are visible quantities of palm trees, as can be respectively testified by points <strong>s</strong>, <strong>p</strong> and <strong>r</strong> on the road. On the other hand, <strong>0</strong> and <strong>1</strong> are not visible quantities, because from every point of the road at least <strong>2</strong> palm trees are visible. Finally, no <strong>m &gt; 4</strong> is a visible quantity, since there are only <strong>4</strong> palm trees in total. Therefore, in this example there are <strong>3</strong> visible quantities of palm trees. (Note that if <strong>m</strong> is a visible quantity of palm trees, there could be more than one point on the road that testifies to this situation; in the previous example this is the case with points <strong>p</strong> and <strong>q</strong> for the visible quantity <strong>3</strong>, as well as with infinitely many other points along with <strong>r</strong> for visible quantity <strong>4</strong>.)</p>
<p>Ana and Adan are getting tired. They want Alan and Amanda to let go of the palm trees and at least prepare some sandwiches. For that reason, you need to make a program to calculate how many different visible quantities of palm trees there are along the road.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer number <strong>N</strong> indicating the number of palm trees that there are on the side of the road (<strong>1 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;1000</strong>). Each of the following <strong>N</strong> lines describes a different palm tree using two integer numbers <strong>X</strong> and <strong>Y</strong>, representing the coordinates of said palm tree in the <strong>XY</strong> plane (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;X, Y&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong>). There are no two palm trees that share the same position.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a single line containing an integer number representing the number of visible quantities of palm trees that there are along the road.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
2 1
3 1
3 2
3 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">7
2 1
3 1
4 1
1 2
3 2
5 2
3 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">4</span><span style="white-space: normal;">
</span></pre>