<p>Andy is a successful farmer. He has a field sized 1 x N tiles, where each tile can be planted a plant. Andy has 26 kind of plants, which is represented by the letter 'a' - 'z'.</p>
<p>Each month Andy has to pay tax to the government. The government in his place is very picky. He wants the tax in the form of a block of tiles. He also demands that the block must contain at least Xi number of plant type Yi. A block of tiles is all the tile from range a to b. To minimize the loss, Andy will pay in the smallest block possible. Help Andy to find the length of the smallest block to satisfy the government.</p>
<h3>Input</h3>
<p>Starts with a number N. The next line is a string of length N containing the letter 'a' to 'z'. The next line is a number K, and for the next K lines are the Xi and Yi, number and type of plants that must be fulfilled.</p>
<h3>Output</h3>
<p>Minimum length of block to pay the tax. If Andy can't pay the tax, output "Andy rapopo".</p>
<h3>Sample Input 1</h3>
<pre>5<br>aabac<br>3<br>1 a<br>1 b<br>1 c</pre>
<h3>Sample Output 1</h3>
<pre>3</pre>
<h3>Sample Input 2</h3>
<pre>5<br>aabac<br>3<br>1 a<br>1 b<br>2 c</pre>
<h3>Sample Output 2</h3>
<pre>Andy rapopo</pre>
<div style="border: 1px solid #FC0; background-color: #ffc; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<ul>
<li>1 ¡Ü N ¡Ü 100000</li>
<li>1 ¡Ü K ¡Ü 26</li>
<li>1 ¡Ü X ¡Ü 100000</li>
<li>Yi is a character from 'a' to 'z'</li>
<li>Each Yi type will not appear more than once</li>
</ul>
</div>
<p><span style="font-weight: bold;">Time limit is very strict, some language might not be able to pass.</span></p>