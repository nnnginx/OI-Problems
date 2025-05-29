<h3>  Pool construction</h3>
<!--l. 3-->
<p>You are working for the International Company for Pool Construction, a construction company which specializes in building swimming pools. A new client wants to build several new pool areas. <!--l. 7--></p>
<p>A pool area is a rectangular grid of <em>w </em>�� <em>h </em>square patches, consisting of zero or more (possibly disconnected) pools. A pool consists of one or multiple connected hole patches, which will later be filled with water. In the beginning, you start with a piece of land where each patch is either a hole in the ground (��.��) or flat grass (��#��). In order to transform this land into a pool area, you must adhere to the following:</p>
<ul>
<li>You can leave a patch as it is. This costs nothing. </li>
<li>If the patch is grass in the beginning, you can dig a hole there. This costs <em>d </em>EUR. </li>
<li>If the patch is a hole in the beginning, you can fill the hole and put grass on top.       This costs <em>f </em>EUR. </li>
<li>You <em>must </em>place special boundary elements along each edge running between a final       grass patch and a final hole patch, to ensure that water does not leak from the pool.       This costs <em>b </em>EUR per boundary element. </li>
<li>The outermost rows and columns of the pool area must always be grass.</li>
</ul>
<!--l. 26-->
<p>You are given the task of calculating the cost of the cheapest possible pool area given the layout of the existing piece of land. <!--l. 29--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 30-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with two integers <em>w </em>and <em>h </em>(2 �� <em>w,h </em>�� 50): the width and height of the       building site. </li>
<li>one line with three integers <em>d</em>, <em>f </em>and <em>b </em>(1 �� <em>d,f,b </em>�� 10<span style="margin-left:0.3em">&nbsp;000): the costs for digging a       new hole, filling an existing hole, and building a boundary element between a pool       and grass patch. </span></li>
<li><em>h </em>lines of <em>w </em>characters each, denoting the layout of the original building site.</li>
</ul>
<!--l. 43-->
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 44-->
<p>Per test case:</p>
<ul>
<li>one line with an integer: the cost of building the cheapest possible pool area from       the original piece of land.</li>
</ul>
<!--l. 51-->
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>3
3 3
5 5 1
#.#
#.#
###
5 4
1 8 1
#..##
##.##
#.#.#
#####
2 2
27 11 11
#.
.#</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>9
27
22 </pre>
</td>
</tr>
</tbody>
</table>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>