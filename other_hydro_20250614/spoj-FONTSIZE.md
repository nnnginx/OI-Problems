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

<div>
	<div class="section">
		<h3>Description</h3>
		<div class="paragraph">
			John bought a billboard. He knows what text he wants to put on it, and he has chosen a monospace font to use, but he doesn't know what the font size should be.
		</div>
		<div class="paragraph">
			Naturally, John wants to use the largest font size possible.
		</div>
		<div class="paragraph">
			Sizing works as follows:
			<ul>
				<li>The height of a line is the font size.</li>
				<li>The width of a character is two-thirds of the font size.</li>
				<li>Lines can only break between the space-separated words.</li>
				<li>If a space ever falls at the beginning or end of a line, it is omitted.</li>
			</ul>
			Don't worry about details like kerning and line spacing.
		</div>
		<div class="paragraph">
			For example, consider the message "The lazy brown dog".
		</div>
		<div class="paragraph">
			On a billboard 60 inches wide and 25 inches tall, the maximum font size is 10 inches:
		</div>
<pre class="center billboard" style="font-size:15px;height:2.5em;width:9ch">The lazy
brown dog</pre>
		<div class="paragraph">
			On a billboard 50 inches wide and 50 inches tall, the maximum size is 12.5 inches:
		</div>
<pre class="center billboard" style="font-size:18.75;height:4em;width:6ch">The
lazy
brown
dog</pre>
		<div class="paragraph">
			Given the size of the billboard and the message, find the largest font size that will allow the entire message to fix.
		</div>
	</div>

	<div class="section">
		<h3>Input</h3>
		<div class="paragraph">
			The first line is the width of the billboard in inches, 0 &lt;= W &lt;= 7500, and the height of the billboard in inches, 0 &lt;= H &lt;= 7500.
			<br>
			The third line is the non-empty message, which is comprised of alphanumeric words separated by single spaces. The message is most 10,000 characters long.
		</div>
	</div>

	<div class="section">
		<h3>Output</h3>
		<div class="paragraph">
			Print the maximum possible font size, in inches. Your answer must be accurate to within 0.001 of the actual value.
		</div>
	</div>

	<table class="section example-table">
		<tbody><tr>
			<th>Input</th>
			<th>Input</th>
		</tr>
		<tr>
			<td>
<pre>60 25
The lazy brown dog</pre>
			</td>
			<td>
<pre>50 50
The lazy brown dog</pre>
			</td>
		</tr>
		<tr>
			<th>Output</th>
			<th>Output</th>
		</tr>
		<tr>
			<td>
<pre>10</pre>
			</td>
			<td>
<pre>12.5</pre>
			</td>
		</tr>
	</tbody></table>
</div>