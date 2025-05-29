<style>
	.center {
		margin-right: auto;
		margin-left: auto;
	}

	.center-text {
		text-align: center ! important;
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

	.inline {
		display: inline;
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

	ul.padded > li, ol.padded > li {
		margin-bottom: 13px;
	}
	ul.padded > li:last-child, ol.padded > li:last-child {
		margin-bottom: 0;
	}

	pre {
		tab-size: 4;
	}

	.billboard {
		line-height: 1em;
		outline: solid 1px black;
	}
</style>

<div>
	<div class="section">
		<h3>Description</h3>
		<div class="paragraph">
			T.E. Lawrence, popularized by the movie <i>Lawrence of Arabia</i>, was a British officer during World War I. He is best known for disrupting the railroads of the Ottoman Empire.
		</div>
		<div class="paragraph">
			For this problem, the railroad of concern runs uninterrupted without branches through several outposts.
<pre class="center-text">P ----- P ----- P ----- P</pre>
		</div>
		<div class="paragraph">
			Each outpost has a value. The strategic value of a group of connected outposts is the sum of the pairwise products of the outposts. A single outpost <pre class="inline">a</pre> has no strategic value; two connected outposts <pre class="inline">a</pre> and <pre class="inline">b</pre> have strategic value <pre class="inline">a*b</pre>; three connected outputs <pre class="inline">a</pre>, <pre class="inline">b</pre>, and <pre class="inline">c</pre> have stategic value <pre class="inline">a*b + a*c + b*c</pre>; and so on.
		</div>
		<div class="paragraph">
			The total stategic value of the railroad is the sum of the strategic values of these connected groups
		</div>
		<div class="paragraph">
			Lawrence can attack and destroy a certain number of railroad segments. His goal is to reduce the strategic value of the railroad as much as possible.
		</div>
		<div class="paragraph">
			For example, consider the following railroad
<pre class="center-text">4 ----- 5 ----- 1 ----- 2</pre>
			The stategic value is 4*5 + 4*1 + 4*2 + 5*1 + 5*2 + 1*2, or 49.
		</div>
		<div class="paragraph">
			Suppose Lawrence has one attack, which is marked by an x.
			<ol class="padded"> 
				<li> 
					He could attack the left segment.
<pre class="center-text">4   x   5 ----- 1 ----- 2</pre>
					The left group has no value, and the right group has value 5*1 + 5*2 + 1*2, for a total of 17.
				</li>
				<li>
					Or he could attack the middle segment.
<pre class="center-text">4 ----- 5   x   1 ----- 2</pre>
					The left group has value 4*5, and the right group has value 1*2, for a total of 22.
				</li>
				<li>
					Or he could attack the right segment.
<pre class="center-text">4 ----- 5 ----- 1   x   2</pre>
					The left group has value 4*5 + 4*1 + 5*1, and the right group has no value, for a total of 29.
				</li>
			</ol>
		</div>
		<div class="paragraph">
			In this case, it would be best for Lawrence to attack the left segment.
		</div>
	</div>

	<div class="section">
		<h3>Input</h3>
		<div class="paragraph">
			The first line is the number of outposts, 0 &lt; P &lt;= 500.
			<br>
			The second line is the number of railroad segments Lawrence can destroy, 0 &lt;= N &lt; P. 
			<br>
			The third line is the space-separated values of the S outposts. Each value is an integer from 0 to 20, inclusive.
		</div>
	</div>

	<div class="section">
		<h3>Output</h3>
		<div class="paragraph">
			The minimum possible stategic value of the railroad after Lawrence's attack.
		</div>
	</div>

	<table class="section example-table">
		<tbody><tr>
			<th>Input</th>
			<th>Input</th>
		</tr>
		<tr>
			<td>
<pre>4
1
4 5 1 2</pre>
			</td>
			<td>
<pre>4
2
4 5 1 2</pre>
			</td>
		</tr>
		<tr>
			<th>Output</th>
			<th>Output</th>
		</tr>
		<tr>
			<td>
<pre>17</pre>
			</td>
			<td>
<pre>2</pre>
			</td>
		</tr>
	</tbody></table>
</div>