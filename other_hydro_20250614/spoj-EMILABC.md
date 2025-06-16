<p>Archeologists have discovered an ancient manuscript describing a big  pyramid. 		The pyramid is built of cubical stone blocks as shown in the picture.  There are <strong>N</strong> horisontal levels in the pyramid. 		The topmost level consists of a single block, and the base level is a  square of <strong>2*N-1¡Á2*N-1</strong> blocks. 		The archeologists  learned from the manuscript the size of a stone  block and the orientation the pyramid. 		However, they do not know the size and the exact location of the  pyramid.</p>
<p>There are many hills in the land where the pyramid is believed to be  located. The archeologists think that one of the hills is actually 		the pyramid covered with sand. To check that hypothesis, they produced  an elevation map of the land. 		The land was divided into a grid of <strong>H¡ÁW</strong> cells. The size of a  cell is the same as the size of a stone block face. 		For each cell they measured its height and calculated how many stone  blocks can be underneath the surface of the cell.</p>
<p>Now the archeologists  give you the elevation map and ask to compute  the largest possible pyramid size, assuming that the pyramid base sides  are parallel to the grid lines.</p>

<h3>Input</h3>
<p>The first line of the input contains two integers <strong>H</strong> and <strong>W</strong> (<strong>0 &lt; H, W ¡Ü 200</strong>).
 Each of the subsequent <strong>H</strong> lines contains <strong>W</strong> integers. Each  integer is non-negative and less than 201.</p>

<h3>Output</h3>
<p>One interger - the number of levels in the larget possible pyramid.</p>

<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>5 6<br>0 0 0 0 0 0<br>0 1 0 0 0 0<br>0 0 1 1 1 1<br>0 0 1 1 2 1<br>0 0 1 1 1 1</pre>

<p><strong>Output:</strong></p>
<pre>2</pre>