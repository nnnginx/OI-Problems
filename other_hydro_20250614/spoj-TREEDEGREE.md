<p>mrm_196 always represents the rooted trees in a simple array, but the array holds four conditions:</p>
<ol>
<li>If the tree has N vertices, the array has length 2N.</li>
<li>Each vertex has a number (from 1 to N) which is written twice (but they may not be necessarily beside each other).</li>
<li>Between the numbers of each vertex, the numbers on its subtree are written.</li>
<li>Vertex 1 is always the root of the tree.</li>
</ol>
<p>For example, he may store the following tree in one of these six ways:</p>
<p><img style="float: left;" src="./24735/file/elJzwezz.png" alt="Sample Tree" width="245" height="206"></p>
<p>&nbsp;</p>
<p>Tree = {1, 3, 2, 2, 4, 4, 5, 5, 3, 1}</p>
<p>Tree = {1, 3, 4, 4, 2, 2, 5, 5, 3, 1}</p>
<p>Tree = {1, 3, 5, 5, 4, 4, 2, 2, 3, 1}</p>
<p>Tree = {1, 3, 2, 2, 5, 5, 4, 4, 3, 1}</p>
<p>Tree = {1, 3, 4, 4, 5, 5, 2, 2, 3, 1}</p>
<p>Tree = {1, 3, 5, 5, 2, 2, 4, 4, 3, 1}</p>
<p>&nbsp;</p>
<p>Your task is pretty simple, find what he always wanted, THE DEGREE OF THE TREE!!!!</p>
<p>Degree of a tree is the maximum degree of all its vertices.</p>
<h3>Input</h3>
<p class="MsoNormalCxSpFirst">The first line of the input contains an integer&nbsp;<em>T</em>&nbsp;(1 ≤ <em>T</em> ≤ 20)&nbsp;— the number tests to answer.</p>
<p class="MsoNormalCxSpMiddle">The first line of each test contains an integer&nbsp;<em>N</em>&nbsp;(1 ≤ <em>N</em> ≤ 100 000)&nbsp;— the number of vertices in the tree.</p>
<p class="MsoNormalCxSpMiddle">The second line of each test contains&nbsp;2<em>N</em>&nbsp;integers&nbsp;<em>a</em><sub>1</sub>, <em>a</em><sub>2</sub>, ..., <em>a<sub>2N</sub></em>&nbsp;(1 ≤ <em>a<sub>i</sub></em> ≤ <em>N</em>) — the elements of his array.</p>
<p class="MsoNormal">It’s guaranteed that the given array always forms at least one valid tree.</p>
<h3>Output</h3>
<p class="MsoNormal">For each test, print a single integer in one line — the degree of the tree.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1
1 1
5
1 3 2 2 4 4 5 5 3 1

<strong>Output:</strong>
0
4
</pre>
<p><strong>Warning: large Input/Output data, be careful with certain languages</strong></p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><!--[if gte vml 1]><v:shapetype id="_x0000_t75"  coordsize="21600,21600" o:spt="75" o:preferrelative="t" path="m@4@5l@4@11@9@11@9@5xe"  filled="f" stroked="f"> <v:stroke joinstyle="miter" /> <v:formulas> <v:f eqn="if lineDrawn pixelLineWidth 0" /> <v:f eqn="sum @0 1 0" /> <v:f eqn="sum 0 0 @1" /> <v:f eqn="prod @2 1 2" /> <v:f eqn="prod @3 21600 pixelWidth" /> <v:f eqn="prod @3 21600 pixelHeight" /> <v:f eqn="sum @0 0 1" /> <v:f eqn="prod @6 1 2" /> <v:f eqn="prod @7 21600 pixelWidth" /> <v:f eqn="sum @8 21600 0" /> <v:f eqn="prod @7 21600 pixelHeight" /> <v:f eqn="sum @10 21600 0" /> </v:formulas> <v:path o:extrusionok="f" gradientshapeok="t" o:connecttype="rect" /> <o:lock v:ext="edit" aspectratio="t" /> </v:shapetype><v:shape id="_x0000_s1026" type="#_x0000_t75" style='position:absolute;  margin-left:0;margin-top:-11.25pt;width:165pt;height:139.1pt;z-index:251658240;  mso-position-horizontal:left;mso-position-horizontal-relative:text;  mso-position-vertical-relative:text'> <v:imagedata src="file:///C:/Users/MOHAMA~1/AppData/Local/Temp/msohtmlclip1/01/clip_image001.jpg" mce_src="file:///C:/Users/MOHAMA~1/AppData/Local/Temp/msohtmlclip1/01/clip_image001.jpg"   o:title="tree" /> <w:wrap type="square" side="right" /> </v:shape><![endif]--><!--[if !vml]--><img src="file:///C:/Users/MOHAMA~1/AppData/Local/Temp/msohtmlclip1/01/clip_image002.jpg" alt="" hspace="12" width="220" height="185" align="left"><!--[endif]--></div>