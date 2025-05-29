<p>Lenka likes to bake cakes since her childhood, when she has learned to bake from her mom.  She soon became a cake expert able to bake chocolate cakes, apple pies, muffins, cookies, cheese cakes, tortes and many other cakes.</p>
<p>Recently, she has started her studies of math at Comenius University in Bratislava.  In the first year she is taking combinatorics class. Today she is studying for the final exam. Since the brain needs a lot of sugar to study math, she has baked, just for herself, her favorite, very delicious, strawberry cake.</p>
<p>The cake, still hot, is lying on an <strong>N</strong>¡Á<strong>M</strong> inch sheet pan.  Hungrily waiting for the cake to cool off Lenka came up with an interesting combinatorial question:  How many different possibilities to cut the cake are there so that every  connected piece consists of some number of 1¡Á1 inch unit squares?</p>
<h3>Problem specification</h3>
<p>The cake can be viewed as a grid consisting of <strong>N</strong>¡Á<strong>M</strong> unit squares. We are allowed to cut the cake along the grid lines. As a result the cake splits into several connected pieces. (Two unit squares remain connected  if they share a side which was not cut.) How many different ways are there to cut the cake?  We consider two cuttings of the cake to be the same if the resulting connected pieces  of both cuttings have the same shape and are at the same positions within the cake. In other words, we are only counting those cuttings where no cut leads between two unit squares that are in the same connected piece.</p>
<p>The following picture ilustrates all the 12 different possible ways how to cut a 2¡Á2 inch cake: <img src="../../../content/john_jones:cake3a.gif" alt="12 possible ways of cutting a 2¡Á2 cake"><br> Note that cutting, for example, as on following picture<br> <img src="../../../content/john_jones:cake3b.gif" alt="Not a good way of cutting"><br> is the same as not cutting at all.</p>
<h3>Input specification</h3>
<p>The first line of the input file contains an integer <strong>T</strong> specifying the number of test cases. Each test case is preceded by a blank line.</p>
<p>Each test case consists of a single line with two positive integers <strong>N</strong> and <strong>M</strong> ¨C dimensions of the cake.</p>
<h3>Output specification</h3>
<p>For each test case output a line with a single positive integer ¨C the number of different possibilities how to cut the cake.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>2

1 2

2 2
</pre>
<p><strong>Output:</strong></p>
<pre>2
12
</pre>
<p><strong>Note</strong></p>
<p>For all the test cases, <em>min</em>(<strong>N</strong>,<strong>M</strong>)&lt;=5, <em>max</em>(<strong>N</strong>,<strong>M</strong>)&lt;=130.</p>