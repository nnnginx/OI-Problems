<style>
	.center {
		margin-right: auto;
		margin-left: auto;
	}

	.example-table {
		margin-top: 10px;
		text-align: left;
		width: 100%;
	}

	.example-table td {
		max-width: 0;
		word-wrap: break-word;
		vertical-align: top; 
	}

	.example-table .vertical-spacer {
		height: 5px;
	}

	.section {
		margin-top: 19px;
		margin-bottom:19px;
	}

	.section:first-child, .section:first-child > h3:first-child {
		margin-top: 0;
	}

	.paragraph {
		margin-top: 10px;
		margin-bottom: 10px;
		text-align: left;
	}

	.paragraph ul, .paragraph pre {
		margin-top: 3px;
		margin-bottom: 3px;
	}

	pre {
		tab-size: 4;
	}

	.billboard {
		line-height: 1em;
		outline: solid 1px black;
	}
</style>

<style>
	svg.example {
		width: 195px;
		height: 195px;
		display: inline-block;
	}

	.bilbo circle {
		stroke: black;
		stroke-width: 1;
		fill: white;
	}
	.bilbo text {
		font-family: sans-serif;
		font-size: .5px;
		font-weight: bold;
		text-anchor: middle;
	}
	.obstacle {
		stroke: black;
		stroke-width: 1;
		fill: none;
		shape-rendering: geometricPrecision;
	}
	.ray {
		stroke: blue;
		stroke-width: 1;
	}
	.grid line {
		stroke: #ccc;
		stoke-width: 1;
	}
</style>

<div>
	<div class="section">
		<h3>Description</h3>
		<div class="paragraph">
			Bilbo the Barrelrider is attempting to elude Smaug the Terrible in the treasure-filled halls of Erebor.
		</div>
		<div class="paragraph">
			He uses the obstacles (piles of gold, columns, etc.) in the room to hide from Smaug's view. These obstacles can be approximated by circles.
		</div>
		<div class="paragraph">
			Smaug may approach Bilbo from any direction. Bilbo's <em>concealment</em> is the proportion of directions for which an obstacle would be between himself and the dragon.
		</div>
		<div class="paragraph">
			In total, how much concealment do the obstacles offer Bilbo?
		</div>
		<div class="paragraph">
			In the example below to the left, the obstacle affords him 90 degrees (25%) concealment.
			<br>
			In the middle example, Bilbo is right next to the obstacle, and it offers 180 degrees (50%) concealment.
			<br>
			If Bilbo is inside an obstacle (say, inside a pile of gold), he cannot be seen at all.
		</div>
		<svg class="example" viewBox="-4.05 -4.05 8.1 8.1">
			<g class="grid">
				<line x1="-4" y1="-10" x2="-4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-3" y1="-10" x2="-3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-2" y1="-10" x2="-2" y2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line x1="-1" y1="-10" x2="-1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="0" y1="-10" x2="0" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="1" y1="-10" x2="1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="2" y1="-10" x2="2" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="3" y1="-10" x2="3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="4" y1="-10" x2="4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-4" x1="-10" y2="-4" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-3" x1="-10" y2="-3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-2" x1="-10" y2="-2" x2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line y1="-1" x1="-10" y2="-1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="0" x1="-10" y2="0" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="1" x1="-10" y2="1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="2" x1="-10" y2="2" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="3" x1="-10" y2="3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="4" x1="-10" y2="4" x2="10" vector-effect="non-scaling-stroke"></line>
			</g>
			<circle class="obstacle" cx="2" cy="-2" r="2" vector-effect="non-scaling-stroke"></circle>
			<line class="ray" x1="0" y1="0" x2="0" y2="-4" vector-effect="non-scaling-stroke"></line>
			<line class="ray" x1="0" y1="0" x2="4" y2="0" vector-effect="non-scaling-stroke"></line>
			<g class="bilbo">
				<circle cx="0" cy="0" r=".3" vector-effect="non-scaling-stroke"></circle>
				<text x="0" y=".18" class="bilbo">B</text>
			</g>
		</svg>
		<svg class="example" viewBox="-4.05 -4.05 8.1 8.1">
			<g class="grid">
				<line x1="-4" y1="-10" x2="-4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-3" y1="-10" x2="-3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-2" y1="-10" x2="-2" y2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line x1="-1" y1="-10" x2="-1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="0" y1="-10" x2="0" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="1" y1="-10" x2="1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="2" y1="-10" x2="2" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="3" y1="-10" x2="3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="4" y1="-10" x2="4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-4" x1="-10" y2="-4" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-3" x1="-10" y2="-3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-2" x1="-10" y2="-2" x2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line y1="-1" x1="-10" y2="-1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="0" x1="-10" y2="0" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="1" x1="-10" y2="1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="2" x1="-10" y2="2" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="3" x1="-10" y2="3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="4" x1="-10" y2="4" x2="10" vector-effect="non-scaling-stroke"></line>
			</g>
			<circle class="obstacle" cx="2" cy="0" r="2" vector-effect="non-scaling-stroke"></circle>
			<line class="ray" x1="0" y1="0" x2="0" y2="-4" vector-effect="non-scaling-stroke"></line>
			<line class="ray" x1="0" y1="0" x2="0" y2="4" vector-effect="non-scaling-stroke"></line>
			<g class="bilbo">
				<circle cx="0" cy="0" r=".3" vector-effect="non-scaling-stroke"></circle>
				<text x="0" y=".18" class="bilbo">B</text>
			</g>
		</svg>
		<svg class="example" viewBox="-4.05 -4.05 8.1 8.1">
			<g class="grid">
				<line x1="-4" y1="-10" x2="-4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-3" y1="-10" x2="-3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-2" y1="-10" x2="-2" y2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line x1="-1" y1="-10" x2="-1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="0" y1="-10" x2="0" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="1" y1="-10" x2="1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="2" y1="-10" x2="2" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="3" y1="-10" x2="3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="4" y1="-10" x2="4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-4" x1="-10" y2="-4" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-3" x1="-10" y2="-3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-2" x1="-10" y2="-2" x2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line y1="-1" x1="-10" y2="-1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="0" x1="-10" y2="0" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="1" x1="-10" y2="1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="2" x1="-10" y2="2" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="3" x1="-10" y2="3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="4" x1="-10" y2="4" x2="10" vector-effect="non-scaling-stroke"></line>
			</g>
			<circle class="obstacle" cx="1" cy="0" r="2" vector-effect="non-scaling-stroke"></circle>
			<g class="bilbo">
				<circle cx="0" cy="0" r=".3" vector-effect="non-scaling-stroke"></circle>
				<text x="0" y=".18px" class="bilbo">B</text>
			</g>
		</svg>
		<div class="paragraph">
			Obstacles can overlap. 
			<br>
			In the example below to the left, Bilbo has 100% concealment.
			<br>
			In the right example, he has 90 + 53.1 = 143.1 degrees (40%) concealment. 
		</div>
		<svg class="example" viewBox="-4.05 -4.05 8.1 8.1">
			<g class="grid">
				<line x1="-4" y1="-10" x2="-4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-3" y1="-10" x2="-3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-2" y1="-10" x2="-2" y2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line x1="-1" y1="-10" x2="-1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="0" y1="-10" x2="0" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="1" y1="-10" x2="1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="2" y1="-10" x2="2" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="3" y1="-10" x2="3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="4" y1="-10" x2="4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-4" x1="-10" y2="-4" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-3" x1="-10" y2="-3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-2" x1="-10" y2="-2" x2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line y1="-1" x1="-10" y2="-1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="0" x1="-10" y2="0" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="1" x1="-10" y2="1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="2" x1="-10" y2="2" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="3" x1="-10" y2="3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="4" x1="-10" y2="4" x2="10" vector-effect="non-scaling-stroke"></line>
			</g>
			<circle class="obstacle" cx="0" cy="-2" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="-1" cy="-1" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="-2" cy="0" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="-1" cy="1" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="0" cy="2" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="1" cy="1" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="2" cy="0" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="1" cy="-1" r="1" vector-effect="non-scaling-stroke"></circle>
			<g class="bilbo">
				<circle cx="0" cy="0" r=".3" vector-effect="non-scaling-stroke"></circle>
				<text x="0" y=".18px" class="bilbo">B</text>
			</g>
		</svg>
		<svg class="example" viewBox="-4.05 -4.05 8.1 8.1">
			<g class="grid">
				<line x1="-4" y1="-10" x2="-4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-3" y1="-10" x2="-3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="-2" y1="-10" x2="-2" y2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line x1="-1" y1="-10" x2="-1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="0" y1="-10" x2="0" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="1" y1="-10" x2="1" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="2" y1="-10" x2="2" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="3" y1="-10" x2="3" y2="10" vector-effect="non-scaling-stroke"></line>
				<line x1="4" y1="-10" x2="4" y2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-4" x1="-10" y2="-4" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-3" x1="-10" y2="-3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="-2" x1="-10" y2="-2" x2="10" vector-effect="non-scaling-stroke"></line>&gt;
				<line y1="-1" x1="-10" y2="-1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="0" x1="-10" y2="0" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="1" x1="-10" y2="1" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="2" x1="-10" y2="2" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="3" x1="-10" y2="3" x2="10" vector-effect="non-scaling-stroke"></line>
				<line y1="4" x1="-10" y2="4" x2="10" vector-effect="non-scaling-stroke"></line>
			</g>
			<circle class="obstacle" cx="2" cy="1" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="3" cy="1" r="1" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="-2" cy="-2" r="2" vector-effect="non-scaling-stroke"></circle>
			<circle class="obstacle" cx="-3" cy="-2" r="1" vector-effect="non-scaling-stroke"></circle>
			<line class="ray" x1="0" y1="0" x2="4" y2="0" vector-effect="non-scaling-stroke"></line>
			<line class="ray" x1="0" y1="0" x2="3" y2="4" vector-effect="non-scaling-stroke"></line>
			<line class="ray" x1="0" y1="0" x2="0" y2="-5" vector-effect="non-scaling-stroke"></line>
			<line class="ray" x1="0" y1="0" x2="-5" y2="0" vector-effect="non-scaling-stroke"></line>
			<g class="bilbo">
				<circle cx="0" cy="0" r=".3" vector-effect="non-scaling-stroke"></circle>
				<text x="0" y=".18px" class="bilbo">B</text>
			</g>
		</svg>
	</div>

	<div class="section">
		<h3>Input</h3>
		<div class="paragraph">
			The first line is 0 &lt;= N &lt;= 1000, the number of obstacles.
			<br>
			The next N lines are the obstacles, each represented by 3 space-separated integers. The first two integers are -5000 &lt;= X &lt;= 5000 and -5000 &lt;= Y &lt;= 5000, which are the x- and y-coordinates, respectively, of the center of the obstacle. (Bilbo is standing at (0,0).) The third integer is its radius 0 &lt; R &lt;= 1000.
		</div>
	</div>

	<div class="section">
		<h3>Output</h3>
		<div class="paragraph">
			Print the percentage of concealment the obstacles offer Bilbo, rounded to the nearest whole percent.
		</div>
	</div>

	<table class="section example-table">
		<tbody><tr>
			<th>Input</th>
			<th>Input</th>
			<th>Input</th>
			<th>Input</th>
			<th>Input</th>
		</tr>
		<tr>
			<td>
<pre>1
2 2 2</pre>
			</td>
			<td>
<pre>1
2 0 2</pre>
			</td>
			<td>
<pre>1
1 0 2</pre>
			</td>
			<td>
<pre>8
0 -1 1
-1 0 1
-2 1 1
-1 2 1
0 -1 1
1 -2 1
2 -1 1
1 0 1</pre>
			</td>
			<td>
<pre>4
-3 2 1
-2 2 2
2 -1 1
3 -1 1</pre>
			</td>
		</tr>
		<tr>
			<th>Output</th>
			<th>Output</th>
			<th>Output</th>
			<th>Output</th>
			<th>Output</th>
		</tr>
		<tr>
			<td>
<pre>25%</pre>
			</td>
			<td>
<pre>50%</pre>
			</td>
			<td>
<pre>100%</pre>
			</td>
			<td>
<pre>100%</pre>
			</td>
			<td>
<pre>40%</pre>
			</td>
		</tr>
	</tbody></table>
</div>