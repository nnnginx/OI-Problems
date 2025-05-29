<p>In the Mines of Moria, the job of Gakrobera Silverborn the dwarf is to load minecarts with <span class="math inline"><em>N</em></span> stones. The stones are numbered, from 1 to <span class="math inline"><em>N</em></span>, and a given minecart can only be loaded with consecutive stones.</p>
<p>Each stone has a weight between 1 kg and 1000 kg, which we assume to be an integer. The optimal load of a mine cart is 2000 kg. The score of a minecart loaded with <span class="math inline"><em>W</em></span> kg of stones is <span class="math inline">(<em>W</em> − 2000)<sup>2</sup></span>. After all stones have been loaded in minecarts, the total score is the sum of the score of each minecart. The lower the total score is, the better it is.</p>
<p>To help Gakrobera, find the best possible way to load minecarts, given the weights of each stone from 1 to <span class="math inline"><em>N</em></span>.</p>
<p>For example, given four stones of 700 kg, Gakrobera will prefer to load them all in a single minecart (total score <span class="math inline">800<sup>2</sup> = 640 000</span>). But given four stones of 800 kg, Gakrobera will prefer to load two minecarts with two stones (total score <span class="math inline">400<sup>2</sup> + 400<sup>2</sup> = 320 000</span>).</p>
<h3 id="input">Input</h3>
<p>The input begins with an integer <span class="math inline"><em>T</em></span> (<span class="math inline">1 ≤ <em>T</em> ≤ 1000</span>), the number of test cases. Then <span class="math inline"><em>T</em></span> test cases follow.</p>
<p>Each test case is a line of space-separated integers. The first integer <span class="math inline"><em>N</em></span> (<span class="math inline">1 ≤ <em>N</em> ≤ 10<sup>6</sup></span>) is the number of stones to be loaded. Next come <span class="math inline"><em>N</em></span> integers <span class="math inline"><em>w</em><sub>1</sub></span>, …, <span class="math inline"><em>w</em><sub><em>N</em></sub></span> (<span class="math inline">1 ≤ <em>w</em><sub><em>i</em></sub> ≤ 1000</span>), where <span class="math inline"><em>w</em><sub><em>i</em></sub></span> is the weight of the stone <span class="math inline"><em>i</em></span>.</p>
<h3 id="output">Output</h3>
<p>For each test case, output the smallest possible total score.</p>
<h3 id="example">Example</h3>
<pre><strong>input</strong>
3
4 700 700 700 700
4 800 800 800 800
10 100 200 300 400 500 600 700 800 900 1000


<strong>output</strong>
640000
320000
270000
</pre>