<p>The story to this problem has trailed off.</p>
<p>Given integers <span class="math inline"><em>n</em></span>, <span class="math inline"><em>m</em></span>, and <span class="math inline"><em>k</em></span>, compute the real number <span class="math inline"><em>n</em><sup>−<em>m</em></sup></span> (also known as <span class="math inline">1/<em>n</em><sup><em>m</em></sup></span>) and write it as a decimal number in base 10. You can assume that it won’t be a repeating decimal – it can be written with finitely many digits followed by infinite zeros. Print the trailing <span class="math inline"><em>k</em></span> digits.</p>
<h4 id="input-english">Input</h4>
<p>The input contains multiple testcases. Their number  <span class="math inline"><em>1 ≤ T ≤ 15 </em></span>is in the first line.</p>
<p>Each test case is a single line containing three integers: <span class="math inline"><em>n</em></span>, <span class="math inline"><em>m</em></span> and <span class="math inline"><em>k</em></span>. (<span class="math inline">1 ≤ <em>n</em> ≤ 10<sup>9</sup>, 1 ≤ <em>m</em> ≤ 10<sup>5</sup>, 1 ≤ <em>k</em> ≤ 9</span>)</p>
<p>It is guaranteed that <span class="math inline"><em>n</em><sup>−<em>m</em></sup></span> is not a repeating decimal.</p>
<h4 id="output-english">Output</h4>
<p>Print the last <span class="math inline"><em>k</em></span> digits of <span class="math inline"><em>n</em><sup>−<em>m</em></sup></span> after which there are only infinite zeros.</p>
<p>If there are less than <span class="math inline"><em>k</em></span> digits after the decimal point, do not print the decimal point. You must always print all <span class="math inline"><em>k</em></span> digits, even if your output has leading zeros.</p>
<h4 id="examples">Examples</h4>
<p>Input:</p>
<pre><code>2<br>2 3 2<br>2 3 5</code></pre>
<p>Output:</p>
<pre><code>25<br>00125</code></pre>
<p><em><span class="math inline">2<sup>−3</sup> = 0.125</span>, so the last two digits are 25.</em></p>
<p><em><span class="math inline">2<sup>−3</sup> = 0000.1250000</span>. Ignoring the infinite zeros at the end and the decimal point, the last 5 digits are 00125.</em></p>