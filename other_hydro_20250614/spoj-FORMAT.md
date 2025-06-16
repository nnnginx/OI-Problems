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
		You have been given formatted text and asked to converted it HTML.
	</div>
	<div class="paragraph">
		Each character may be formatted as bold, italic, underlined, or some combination.
	</div>
	<div class="paragraph">
		In HTML, content between <b>&lt; b &gt;</b> and <b>&lt; / b &gt;</b> tags is bold. Content between <i> and </i> tags is italic. Content between <b>&lt; u 

&gt;</b> and <b>&lt; / u &gt;</b> tags is underlined.
	</div>
	<div class="paragraph">
		What is the minimum number of properly nested HTML tags needed to produce a given format?
	</div>
	<div class="paragraph">
		For example, say we wanted to format <b>&lt; i &gt;</b><b>&lt; b &gt;</b>LookAt<b>&lt; / b &gt;</b>Me<b>&lt; / i &gt;</b>!
		<ul>
			<li><b>&lt; b &gt;</b><b>&lt; i &gt;</b>LookAt<b>&lt; / b &gt;</b>Me<b>&lt; / i &gt;</b>! has incorrectly nested tags.</li>
			<li><b>&lt; b &gt;</b><b>&lt; i &gt;</b>LookAt<b>&lt; / i &gt;</b><b>&lt; / b &gt;</b><b>&lt; i &gt;</b>Me<b>&lt; / i &gt;</b>! has correctly nested tags, but is longer 

than necessary.</li>
			<li><b>&lt; i &gt;</b><b>&lt; b &gt;</b>LookAt<b>&lt; / b &gt;</b>Me<b>&lt; / i &gt;</b>! is the shortest and uses the fewest number of tags.</li>
		</ul>
	</div>
</div>

<div class="section">
	<h3>Input</h3>
	<div class="paragraph">
		There will be a sequence of 1 to 20,000 numerals. Each numeral denotes the formatting at that position.
		<ul>
			<li>0 - no formatting</li>
			<li>1 - bold</li>
			<li>2 - italic</li>
			<li>3 - bold and italic</li>
			<li>4 - underlined</li>
			<li>5 - bold and underlined</li>
			<li>6 - italic and underlined</li>
			<li>7 - bold, italic, and underlined</li>
		</ul>
		(There is no need to actually specify the content, since that will not affect the answer.)
		<br>
		The example earlier would be given as 333333220.
	</div>
</div>

<div class="section">
	<h3>Output</h3>
	<div class="paragraph">
		The minimum number of <b>&lt; b &gt;</b>, <b>&lt; / b &gt;</b>, <b>&lt; i &gt;</b>, <b>&lt; / i &gt;</b>, <b>&lt; u &gt;</b>, and <b>&lt; / u &gt;</b> tags required.
	</div>
</div>

<table class="section example-table">
	<tbody><tr>
		<th>Input</th>
		<th>Input</th>
		<th>Input</th>
		<th>Input</th>
	</tr>
	<tr>
		<td>
<pre>01</pre>
		</td>
		<td>
<pre>333333220
</pre>
		</td>
		<td>
<pre>00110066</pre>
		</td>
		<td>
<pre>12364012375303657213412303</pre>
		</td>
	</tr>
	<tr>
		<th>Output</th>
		<th>Output</th>
		<th>Output</th>
		<th>Output</th>
	</tr>
	<tr>
		<td>
<pre>2</pre>
		</td>
		<td>
<pre>4</pre>
		</td>
		<td>
<pre>6</pre>
		</td>
		<td>
<pre>54</pre>
		</td>
	</tr>
</tbody></table>