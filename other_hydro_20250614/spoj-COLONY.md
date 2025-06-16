<style>
	.example-table {
		text-align: left;
		margin-top: 10px;
		width: 100%;
	}

	.example-table td {
		vertical-align: top; 
	}

	.section {
		margin-top: 19px;
		margin-bottom:19px;
	}

	.paragraph {
		text-align: left;
		margin-top: 10px;
		margin-bottom: 10px;
	}

	.paragraph ul, .paragraph ol {
		margin-top: 3px;
		margin-bottom: 3px;
	}
</style>

<div class="section">
	<h3>Description</h3>
	<div class="paragraph">
		Linearians are pecurliar creatures. They are odd in several ways:
		<ol>
			<li>
				Every Linearian is either red or blue.
			</li>
			<li>
				A Linearian colony is a straight line, aligned N-S with the magentic field.
			</li>
			<li>
				A colony starts with single red Linearian.
			</li>
			<li>
				Every year, each Linearian produces an offspring of the opposite color. After birth, the parent moves just south of the offspring. (Since everyone is born at once, this does make for a lot of jostling, but everyone stays in order.)			
			</li>
		</ol>
	</div>
	<div class="paragraph">
		So a colony grows as follows:
	</div>
	<div class="paragraph" style="padding-left:2em">
<pre>N ----------- S

Year 0: R
Year 1: BR
Year 2: RBBR
Year 3: BRRBRBBR
Year 4: RBBRBRRBBRRBRBBR</pre>
	</div>
	<div class="paragraph">
		Given a year and a position along the N-S axis, determine what the color of the Linearian there will be.
	</div>
</div>

<div class="section">
	<h3>Input</h3>
	<div class="paragraph">
		The first line is the year Y (0 &lt;= Y &lt;= 51).
		The second line is the position P from north to south, 0-indexed (0 &lt;= P &lt; 2^Y).
	</div>
</div>

<div class="section">
	<h3>Ouput</h3>
	<div class="paragraph">
		The color of the Linearian, either red or blue.
	</div>
</div>

<table class="section example-table">
	<tbody><tr>
		<th>Input</th>
		<th>Input</th>
	</tr>
	<tr>
		<td>
<pre>3
6</pre>
		</td>
		<td>
<pre>51
123456789012345</pre>
		</td>
	</tr>
	<tr>
		<th>Output</th>
		<th>Output</th>
	</tr>
	<tr>
		<td>
<pre>blue</pre>
		</td>
		<td>
<pre>red</pre>
		</td>
	</tr>
</tbody></table>