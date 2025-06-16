<p><em>This problem is similar but not identical to the problem <a href="../../MORIA">MORIA</a>.</em></p>
<p>In the Mines of Moria, the job of Gakrobera Silverborn the dwarf is still to load minecarts with <span class="math inline"><em>N</em></span> stones. The stones are numbered, from 1 to <span class="math inline"><em>N</em></span>, and a given minecart can only be loaded with consecutive stones.</p>
<p>The minecart have an optimal load <span class="math inline"><em>L</em></span>.<a id="fnref1" class="footnote-ref" href="#fn1"><sup>1</sup></a> Each stone has an integer weight between 1 kg and <span class="math inline"><em>L</em></span> kg. The score of a minecart loaded with <span class="math inline"><em>W</em></span> kg of stones is <span class="math inline">(<em>W</em> − <em>L</em>)<sup>2</sup></span>. After all stones have been loaded in minecarts, the total score is the sum of the score of each minecarts. The lower the total score is, the better it is.</p>
<p>To help Gakrobera, find the best possible way to load minecarts, given the weights of each stone from <span class="math inline">1</span> to <span class="math inline"><em>N</em></span>.</p>
<p>For example, with an optimal load <span class="math inline"><em>L</em> = 2000 kg</span>, given four stones of 700 kg, Gakrobera will prefer to load them all in a single minecart (total score <span class="math inline">800<sup>2</sup> = 640 000</span>). But given four stones of 800 kg, Gakrobera will prefer to load two minecarts with two stones (total score <span class="math inline">400<sup>2</sup> + 400<sup>2</sup> = 320 000</span>).</p>
<p>Beware: the situation in the Mines of Moria has gone wild, the Dwarves push cupidity too far, the optimal load can be very high! The Balrog will soon be awaken…</p>
<h3 id="input">Input</h3>
<p>The input begins with an integer <span class="math inline"><em>T</em></span> (<span class="math inline">1 ≤ <em>T</em> ≤ 1000</span>), the number of test cases. Then <span class="math inline"><em>T</em></span> test cases follow.</p>
<p>Each test case is a line of space-separated integers. The first integer <span class="math inline"><em>L</em></span> (<span class="math inline">1 ≤ <em>L</em> ≤ 10<sup>6</sup></span>) is the optimal load. The second integer <span class="math inline"><em>N</em></span> (<span class="math inline">1 ≤ <em>N</em> ≤ 10<sup>6</sup></span>) is the number of stones to be loaded. Next come <span class="math inline"><em>N</em></span> integers <span class="math inline"><em>w</em><sub>1</sub></span>, …, <span class="math inline"><em>w</em><sub><em>N</em></sub></span> (<span class="math inline">1 ≤ <em>w</em><sub><em>i</em></sub> ≤ 1000</span>), where <span class="math inline"><em>w</em><sub><em>i</em></sub></span> is the weight of the stone <span class="math inline"><em>i</em></span>.</p>
<h3 id="output">Output</h3>
<p>For each test case, output the smallest possible total score.</p>
<h3 id="example">Example</h3>
<pre><strong>input</strong>
3
2000 4 700 700 700 700
2000 4 800 800 800 800
2000 10 100 200 300 400 500 600 700 800 900 1000

<strong>output</strong>
640000
320000
270000
</pre>
<p>
</p><hr>
<ol>
<li id="fn1">
<p>Compared to the situation in the problem <a href="../../MORIA">MORIA</a>, the optimal load is not fixed.<a class="footnote-back" href="#fnref1">↩︎</a></p>
</li>
</ol><p></p>