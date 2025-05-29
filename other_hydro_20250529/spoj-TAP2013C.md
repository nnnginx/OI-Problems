<p><em><strong>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</strong></em></p>
<p>Once upon a time there was a very joyous girl who was called Little Red-Cap because she always wore a red riding cap. Red-Cap enjoyed a lot her strolls in the woods, during which she collected berries in her small basket to offer them to her grandmother, who was known to prepare the most delicious pies of all the region. However, Red-Cap definitely did not enjoy the perils of the woods, and in particular the Big Bad Wolf who was always hungry and prying.</p>
<p>One day, Red-Cap decides to go from her home to that of her grandmother, collecting berries on the way and trying to make her journey in the safest possible way. Red-Cap's house is in a clearing at the westernmost point of the woods, her grandmother's house is in another clearing at the easternmost point, and inside the woods between them there are some other clearings containing berry trees. The woods are very dense, so the only way to go through them is using the pathways between the clearings, which fortunately Red-Cap knows very well. In order not to get lost, Red-Cap always moves through pathways that take her to a point strictly to the east of the point where she is. In order not to be caught by the wolf Red-Cap finds it imperative to avoid an ambush, and for that reason she always has in mind the number of different paths that take her from her current position to her grandmother's home.</p>
<p>A <em>path </em>in the woods is a sequence of clearings ordered from west to east, such that each clearing is connected with the next by a pathway. A<em> path to the house of Red-Cap's grandmother</em> is simply a path whose last clearing contains said house. For each clearing, its <em>level of alternatives</em> is the number of paths that go from it to Red-Cap's grandmother's house. In turn, for each path its <em>level of alternatives</em> is the sum of the levels of alternatives of all the clearings that make up that path. In order not to be captured by the wolf, Red-Cap wants to find the path with a maximum level of alternatives, starting at her house and ending at her grandmother's house. Can you help her?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integer numbers <strong>N</strong> and <strong>S</strong> which respectively indicate the number of clearings and the number of pathways in the woods (<strong>3 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;3 ��&nbsp;10<sup>4</sup></strong> and <strong>2&nbsp;</strong><strong>��</strong><strong>&nbsp;S&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong>). The clearings are identified by different integer numbers between <strong>1</strong> and <strong>N</strong>, and are ordered from west to east, so that if <strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;i &lt; j&nbsp;</strong><strong>��</strong><strong>&nbsp;N</strong> then clearing <strong>i</strong> is to the west of clearing <strong>j</strong>. Red-Cap's house is in clearing <strong>1</strong>, whereas her grandmother's house is in clearing <strong>N</strong>.</p>
<p>Each of the following <strong>S</strong> lines describes a pathway using two integer numbers <strong>I</strong> and <strong>J</strong>, which indicate that there is a pathway between clearing <strong>I</strong> and clearing <strong>J</strong> (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;I &lt; J&nbsp;</strong><strong>��</strong><strong>&nbsp;N</strong>). There is at least one path from Red-Cap's house to her grandmother's house, and the maximum level of alternatives among the set of all such paths is no greater than <strong>10<sup>18</sup></strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a single line containing an integer number, representing the maximum level of alternatives for a path from Red-Cap's house to her grandmother's house.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3 2
1 2
2 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4 6
1 2
2 3
3 4
1 2
2 3
3 4</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">15</span></pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">9 9
1 3
2 3
3 4
4 5
1 5
3 4
3 9
7 8
4 9</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">8</span><span style="white-space: normal;">
</span></pre>