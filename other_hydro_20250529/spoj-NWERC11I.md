<h3>  Tracking RFIDs</h3>
<!--l. 3-->
<p>Jeroen operates a warehouse storage facility for the North Western Electrical Resource Company (NWERC). When a customer places an order with NWERC, this order is conveyed to the warehouse. Jeroen¡¯s task is to then find the products ordered, pack them into a box, and ship them to the customer. <!--l. 8--></p>
<p>NWERC has an unusual warehouse policy: the products are not arranged in any particular order, and are strewn all over the place. However, it is possible for Jeroen to do his job because each product is tracked using RFID technology<a id="fn1x0-bk" href="#fn1x0"><sup>1</sup></a>. Specifically, each product is assigned a wireless RFID chip as soon as it enters the warehouse, and sensors located on the warehouse ceiling are used to automatically track the products. <!--l. 16--></p>
<p>By default, each sensor has a range of <em>r </em>units ¨C that is, it can read any RFID chip that is located at most <em>r </em>units from it in a straight line. However, if the line segment between a sensor and a product intersects with or touches <em>x </em>walls, the range of the sensor is reduced by <em>x </em>units in that direction. Furthermore, the sensors may fail to read an RFID chip due to interference from other sensors, so the distance between any pair of sensors in the warehouse is guaranteed to be at least <em>r </em>units. You may further assume that no sensor or product is placed on a wall. <!--l. 25--></p>
<p>Jeroen now wants to determine, for each product, which sensors can read its RFID chip. Can you help him? <!--l. 28--></p>
<p>&nbsp;</p>
<hr>
<div id="x1-10021">
<div>
<p><!--l. 30--></p>
<p></p><center><img src="/NWERC11/content/problemI0x.png" alt="PIC" width="383.63158pt" height="210.78658pt"><!--tex4ht:graphics   name="/NWERC11/content/problemI0x.png" src="circles.eps"   --></center><p></p>
</div>
<br>
<div>Figure&nbsp;1: Illustration of sensors, walls and products as in the Sample Input.</div>
<!--tex4ht:label?: x1-10021 --> <!--l. 33-->
<p>&nbsp;</p>
</div>
<hr>
<h4>Input</h4>
<!--l. 36-->
<p>On the first line one positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with four integers <em>s </em>(1 ¡Ü <em>s </em>¡Ü 250<span style="margin-left:0.3em">&nbsp;000), <em>r </em>(1 ¡Ü <em>r </em>¡Ü 25), <em>w </em>(0 ¡Ü <em>w </em>¡Ü 10)       and <em>p </em>(1 ¡Ü <em>p </em>¡Ü 10<span style="margin-left:0.3em">&nbsp;000) where <em>s </em>represents the number of sensors, <em>r </em>the range of each       sensor, <em>w </em>the number of walls and <em>p </em>the number of products. </span></span></li>
<li><em>s </em>lines containing two integers <em>x</em><sub>i</sub> and <em>y</em><sub>i</sub> (-10<span style="margin-left:0.3em">&nbsp;000 ¡Ü <em>x</em><sub>i</sub><em>,y</em><sub>i</sub> ¡Ü 10<span style="margin-left:0.3em">&nbsp;000). Each such line       represents a sensor at location (<em>x</em><sub>i</sub>, <em>y</em><sub>i</sub>). The distance between any pair of sensors is       guaranteed to be at least <em>r </em>units. </span></span></li>
<li><em>w </em>lines containing four integers <em>bx</em><sub>i</sub>, <em>by</em><sub>i</sub>, <em>ex</em><sub>i</sub> and <em>ey</em><sub>i</sub> (-10<span style="margin-left:0.3em">&nbsp;000 ¡Ü <em>bx</em><sub>i</sub><em>,by</em><sub>i</sub><em>,ex</em><sub>i</sub><em>,ey</em><sub>i</sub> ¡Ü 10<span style="margin-left:0.3em">&nbsp;000). Each such line represents a wall, which should be considered as straight line       segment from (<em>bx</em><sub>i</sub>, <em>by</em><sub>i</sub>) to (<em>ex</em><sub>i</sub>, <em>ey</em><sub>i</sub>). The length of this line segment will be positive. </span></span></li>
<li><em>p </em>lines, each containing two integers <em>px</em><sub>i</sub> and <em>py</em><sub>i</sub> (-10<span style="margin-left:0.3em">&nbsp;000 ¡Ü <em>px</em><sub>i</sub><em>,py</em><sub>i</sub> ¡Ü 10<span style="margin-left:0.3em">&nbsp;000). Each       such line represents a product at location (<em>px</em><sub>i</sub>, <em>py</em><sub>i</sub>).</span></span></li>
</ul>
<!--l. 58-->
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 59-->
<p>Per test case:</p>
<ul>
<li><em>p </em>lines, each representing a product in the order they appear in the input. Each       line should contain an integer <em>t</em>, the number of sensors that can track the product;       this integer should then be followed by a list of <em>t </em>ordered pairs representing the       corresponding sensor locations. If there are multiple sensors, they should be sorted       in increasing order by <em>x</em>-coordinate. If multiple sensors have the same <em>x</em>-coordinate,       they should be sorted in increasing order by <em>y</em>-coordinate.</li>
</ul>
<!--l. 71-->
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
<pre>1
4 3 4 7
0 0
-1 3
2 3
11 5
-4 -1 5 -1
3 5 6 1
11 4 11 3
12 5 12 8
1 1
0 -2
4 4
11 2
13 5
13 7
14 5</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>3 (-1,3) (0,0) (2,3)
1 (0,0)
0
0
1 (11,5)
0
0</pre>
</td>
</tr>
</tbody>
</table>
<hr>
<p><a id="fn1x0" href="#fn1x0-bk"><sup>1</sup></a>Objects, that have a radio-frequency identification (RFID) tag attached, can be tracked using radio waves.</p>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>