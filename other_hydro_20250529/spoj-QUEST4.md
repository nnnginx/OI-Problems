<p align="left">
To reach the treasure, <b>Jones</b> has to pass through the <b>"Room of Death"</b>. The floor of this room is a square with side <b>120</b> units. It is laid with square tiles of dimensions <b>{1 X 1}</b> arranged into a grid. But, at some places in the grid tiles are missing. As soon as the door to this room is opened poisonous gas starts coming out of these missing grid locations. The only escape from this gas is to completely cover these locations with planks lying outside the room. Each plank has dimensions <b>{120 X 1}</b> and can only be placed parallel to either sides of the floor. Now <b>Jones</b> wants to minimize the damage to his health so that he has enough of it left for the treasure. He figures out that in order to achieve this he has to use the minimum number of planks possible. He also realises that even if the planks overlap, poisonous gas from the missing tiles can still be successfully blocked. Please help <b>Jones</b> in this task.
</p>

<p align="center">
</p><center>
</center><table><tbody><tr>
	<td><img src="/content/adrian:quest4_1.jpg" width="430" height="486" border="0" alt="Dungeon of Death: Tiles Uncovered"></td></tr><tr>
	<td><img src="/content/adrian:quest4_2.jpg" width="430" height="486" border="0" alt="Dungeon of Death: Tiles Covered"></td>
</tr>
</tbody></table> 
<p></p>

<h3>Input</h3>

<ul> 
	<li> The first line of the input is a positive integer <b>t &lt;= 20</b>, denoting the number of rooms.
	</li><li> The descriptions for the t rooms follow one after the other.
	</li><li> <b>Room Description:</b>
		<ul> 
			<li> The first line of the room description is a positive integer <b>n (n  &lt;=  10010)</b>, denoting the number of missing tile locations.
			</li><li> This is followed by the <b>n</b> lines, one for each missing tile location.
			</li><li> Each line contains two integers <b>x y (0 &lt;= x, y &lt; 120)</b>, separated by a single space, representing the co-ordinates of the missing tile location.
		</li></ul>
</li></ul> 
<p></p>

<h3>Output</h3>
<p>The output should consist of <b>t</b> lines, one for each room. The <b>k<sup>th</sup></b> line in the output should be an integer <b>m<sub>k</sub></b>, the minimum number of planks needed for the <b>k<sup>th</sup></b> room.
</p>

<h3>Example</h3>

<tt>
<p>
<b>Input:</b>
<br>2
<br>3
<br>1 0
<br>2 0
<br>3 0
<br>4
<br>1 1
<br>2 2
<br>3 3
<br>4 4
</p>
<p>
<b>Output:</b>
<br>1
<br>4
</p>
</tt>