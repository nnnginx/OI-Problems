<h4 id="task-english">Task</h4>
<p>You decided to start an online dating site for mathematical objects. Every set, number, algebraic structure and lemma can register on your site and start describing its good qualities in its profile.</p>
<p>This is especially easy for numbers which directly describe themselves when you read them. For example, the number <strong>10123133</strong> contains <strong>one</strong> “<strong>0</strong>”, <strong>one</strong> “<strong>2</strong>”, <strong>three</strong> “<strong>1</strong>”s and <strong>three</strong> “<strong>3</strong>”s. We call numbers like that <em>self describing numbers</em>, and they are very popular.</p>
<p>A bit more formally, an integer is a self-describing number if we can split it into pairs of ((count, digit), (count, digit), (count, digit), …) where for every (count, digit) pair, our number really contains that digit that many times. All counts must be written without leading zeros and all digits appearing in the number must be specified exactly once.</p>
<p>However, the digit <span class="math inline"><em>f</em></span> has fallen out of fashion. Any number that contains the digit <span class="math inline"><em>f</em></span> has no chance.</p>
<p>Consider all self-describing numbers that don’t contain the forbidden digit <span class="math inline"><em>f</em></span>. Print the <span class="math inline"><em>n</em></span>-th smallest such number. (The first <span class="math inline"><em>n</em> − 1</span> self describing numbers are out of your league.)</p>
<h4 id="input-english">Input</h4>
<p>The input contains multiple testcases. Their number <em>1 <span>≤ T <span>≤ 5<span> </span></span></span></em><span><span><span>is on the first line.<br></span></span></span><em><span></span></em></p>
<p>Each testcase is a single line with two integers <span class="math inline"><em>n</em></span> and <span class="math inline"><em>f</em></span>, where <span class="math inline">1 ≤ <em>n</em> ≤ 10<sup>9</sup></span> and <span class="math inline">0 ≤ <em>f</em> ≤ 9</span>.</p>
<h4 id="output-english">Output</h4>
<p>Print the <span class="math inline"><em>n</em></span>-th smallest self describing number that doesn’t contain the digit <span class="math inline"><em>f</em></span>.</p>
<p>The input will be chosen so that the answer always exists.</p>
<h4 id="examples">Examples</h4>
<p>Input:</p>
<pre><code>2<br>1 1<br>1 2<br></code></pre>
<p>Output:</p>
<pre><code>22<br>10143133<br></code></pre>
<p><em>The number 22 is self describing – we can split it as ((2,2)). It is the smallest self describing number that doesn’t contain the digit 1.</em></p>
<p><em>We can read 10143133 as <span class="math inline">((1, 0),(1, 4),(3, 1),(3, 3))</span>. This is the smallest self describing number that doesn’t contain the digit 2.</em></p>