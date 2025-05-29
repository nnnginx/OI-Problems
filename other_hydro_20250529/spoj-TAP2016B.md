<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>&nbsp;</p>
<p>The baking festival has arrived in town. This is a great opportunity for small businesses in the baking industry to collect some money and promote themselves. Each small business wanting to take part in the festival can do so by setting up a small stand in the hall where it takes place. For security reasons, each stand should be placed against one of the hall's walls. In its stall, each business can show its products and make the necessary arrangements to sell them to the public attending the festival. One important characteristic of the stands is that they offer a free sample of some products to whomever may want one. The goal is to show the great quality of the recipes and thus tempt passersby to buy at that stand.</p>
<p>The free samples bring a lot of people to the festival, wanting to eat the delicious desserts for no cost at all as they move around the hall. Most attendees buy some of the products to help the business who really deserve recognition. One of the festival's most famous visitors is Mr. Belly, who always goes by every single stand checking out the free samples, even going as far as giving a prize to the best of them all.</p>
<p>Mr. Belly doesn't want to waste too much time at the festival, so he would like to taste the free samples in all of the stands walking the least possible distance. In order to do this, he has the map printed on the festival's brochure, which was published in advance by the organizers. The map has a drawing of the shape of the hall, which in this case is a convex polygon. It also has markings for <strong>N</strong>&nbsp;important sites, two of which correspond to the entrance and exit of the hall, the other <strong>N-2</strong>&nbsp;being the festival's stands. Each important site is represented by a point on the boundary of the polygon representing the hall's walls.</p>
<p>Mr. Belly is now asking for you to help him complete his mission. He will provide you with the coordinates in the Cartesian <strong>(X, Y)</strong>&nbsp;plane of the <strong>N&nbsp;</strong>important sites in the hall, in counter-clockwise order (<em>i.e.</em>&nbsp;in the order in which he would visit them if he were to go through the hall keeping his right hand on its interior wall). He would like to know what's the minimum distance he must travel in order to visit all the stands, if he is to start at the entrance of the hall, finish at its exit and choose optimally the order in which he visits the stands.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains three integer numbers <strong>N</strong>, <strong>E</strong>&nbsp;and <strong>S</strong>. The integer <strong>N</strong>&nbsp;represents the number of important sites marked on the map, which are numbered from <strong>1</strong>&nbsp;to <strong>N</strong>&nbsp;(<strong>2 ¡Ü&nbsp;N&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;4000</strong>). The integers <strong>E</strong>&nbsp;and <strong>S</strong>&nbsp;represent the numbers of the sites corresponding to the hall's entrance and its exit, respectively (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;E, S&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;N</strong>&nbsp;with <strong>E ¡Ù&nbsp;S</strong>). Each of the following <strong>N</strong>&nbsp;lines contains two integers <strong>X&nbsp;</strong>and <strong>Y</strong>, representing the numbers on the <strong>i</strong>-th line the coordinates <strong>(X, Y)</strong>&nbsp;of the <strong>i</strong>-th important site (<strong>-10<sup>4</sup>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;X, Y&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>4</sup></strong>). All the important sites are located in different points, and there always exists a convex polygon containing all of them in its boundary.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line containing one rational number, representing the minimum distance Mr. Belly needs to walk in order to visit all of the festival's stands, starting at the entrance of the hall and finishing at its exit. Print the result with exactly <strong>6</strong>&nbsp;digits after the decimal marker, rounding if necessary.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">6 1 6
1 0
2 0
3 1
2 2
1 2
0 1
6 1 4
0 0
10 0
20 0
20 1
10 1
0 1</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">6.242641
23.000000</span></pre>