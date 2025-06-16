<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MNERED/en/">English</a></td>
<td width="50%"><a href="/problems/MNERED/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>&nbsp;</p>
<p>In the nearby kindergarten they recently made up an attractive game  of strength and agility that kids love. The surface for the game is a large flat area divided into N¡ÁN squares. The children lay large spongy cues onto the surface. The sides of the cubes are the same length as the sides of the squares. When a cube is put on  the surface, its sides are aligned with some square. A cube may be put  on another cube too. Kids enjoy building forts and hiding them, but they  always leave behind a huge mess. Because of this, prior to closing the  kindergarten, the teachers rearrange all the cubes so that they occupy  a rectangle on the surface, with exactly one cube on every square in the rectangle. In one moving, a cube is taken off the top of a square to the top of any other square.</p>
<p>Write a program that, given the state of the surface, calculates the  smallest number of moves needed to arrange all cubes into a rectangle.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line contains the integers N and M (1 ¡Ü N ¡Ü 100, 1 ¡Ü M ¡Ü N^2),  the dimensions of the surface and the number of cubes currently on the  surface.</p>
<p>Each of the following M lines contains two integers R and C (1 ¡Ü R, C ¡Ü N), the coordinates of the square that contains the cube.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>Output the smallest number of moves. A solution will always exist.</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>input<br>4 3<br>2 2<br>4 4<br>1 1<br>output<br>2<br><br>input<br>5 8<br>2 2<br>3 2<br>4 2<br>2 4<br>3 4<br>4 4<br>2 3<br>2 3<br>output<br>3<br><br>In the second example, a cube is moved from (2, 3) to (3, 3), from (4, 2)<br>to (2, 5) and from (4, 4) to (3, 5).<br></pre>
<p> </p>