<p>
To get to the treasure, <b>Jones</b> must complete one more task. He comes across a table, where there are a number of wooden planks lying along the length of the table. He notices that the width of the table is exactly equal to the width of every plank on it. The planks are so heavy that they cannot be manually moved in any way. Some of these wooden planks are overlapping. <b>Jones</b> has a hammer and the Gods grant him infinite nails. The planks have to be joined to the table with nails such that every plank is connected to the table through at least one nail.  The nails are of sufficient length, and have to be hammered vertically into the table. One or more planks can be joined to the table through a single nail provided they have a common overlap. Find out the minimum number of nails he needs to nail all planks to the table.
</p>

<p align="center"></p><center>
<img src="/content/adrian:quest5.jpg" width="500" border="0" alt="Planks"></center>
<p></p>

<h3>Input</h3>

<ul>
	<li> The first line of the input is a positive integer <b>t &lt;= 20</b>, denoting the number of tables.
	</li><li> The descriptions of the table follow one after the other.

	</li><li> <b>Table description:</b>
	<ul>
	
		<li> The first line of the description of the <b>k<sup>th</sup></b> table contains a positive integer <b>n (n &lt;= 10010)</b>, the number of planks on it. 
		</li><li> This is followed by <b>n</b> lines containing the description of the planks.
		</li><li> The description of each plank is a pair of integers <b>a</b> and <b>b</b> <b>(0 &lt;= a &lt;= b &lt;= 10000010)</b>, denoting the distance of the left end and right end of the plank from the left end of the table.
	</li></ul>
</li></ul>
<p></p>

<h3>Output</h3>
<p>The output must contain <b>t</b> lines , the <b>k<sup>th</sup></b> line corresponding to the <b>k<sup>th</sup></b> table.
The output on the <b>k<sup>th</sup></b> line must be an integer <b>i<sub>k</sub></b>, the minimum number of nails required.
</p>

<h3>Example</h3>
<tt>
<p align="left"><b>Input:</b>
<br>2
<br>3
<br>1 5
<br>3 5
<br>2 4
<br>2
<br>1 4 
<br>4 5
</p>

<p align="left">
<b>Output:</b>
<br>1
<br>1
</p>
</tt>