<p>Kubík went to buy a pizza. To his surprise, the pizza box was made out of recycled… punch cards!</p>
<p>With his eagle eye, he deciphered the program the punch cards described:</p>
<pre><code>n = read_input();
ans = 0;
while(n &gt; 0)
{
    ans = ans + 1;
    n = random() % n;
}</code></pre>
<p><span class="math inline"><em>r</em><em>a</em><em>n</em><em>d</em><em>o</em><em>m</em>()</span> is a function which returns uniformly random non-negative integers, and % is the modulus operator.</p>
<p>Now he wonders what the expected value of <span class="math inline"><em>a</em><em>n</em><em>s</em></span> would be for a given initial value of <span class="math inline"><em>n</em></span>, and he is unable to enjoy his pizza until someone computes the answer for him.</p>
<h4 id="input-english">Input</h4>
<p>The first line contains an integer <strong>1 ≤</strong> <strong>T ≤ 5</strong> - the number of test cases.</p>
<p>Each of the next <strong>T</strong> lines contain a single integer <strong><span class="math inline"><em>n</em></span></strong>, where <strong><span class="math inline">1 ≤ <em>n</em> ≤ 300 000</span></strong>. The sum of <strong>n</strong> within an input file won't exceed 300000.</p>
<h4 id="output-english">Output</h4>
<p>Output the expected value of the variable <strong><span class="math inline"><em>a</em><em>n</em><em>s</em></span></strong> – that is, the sum of <span class="math inline"><strong><em>v</em></strong> × </span>(probability that <strong><span class="math inline"><em>a</em><em>n</em><em>s</em></span></strong> will end up with value <strong><span class="math inline"><em>v</em></span></strong>), for all possible values <strong><span class="math inline"><em>v</em></span></strong>.</p>
<p>Your answer will be considered correct if the absolute or relative error does not exceed <strong><span class="math inline">10<sup>−9</sup></span></strong>. Make sure to print enough decimal places.</p>
<h4 id="examples">Example</h4>
<p><strong>Input:</strong></p>
<pre><code>2
2
47</code></pre>
<p><strong>Output:</strong></p>
<pre><code>1.5
4.4379638417

</code></pre>
<p><em>In the first case, either <span class="math inline"><em>r</em><em>a</em><em>n</em><em>d</em><em>o</em><em>m</em>()%2 = 0</span> with probability <span class="math inline">1/2</span>, which leads to <span class="math inline"><em>a</em><em>n</em><em>s</em> = 1</span>, or <span class="math inline"><em>r</em><em>a</em><em>n</em><em>d</em><em>o</em><em>m</em>()%2 = 1</span> with probability <span class="math inline">1/2</span>, after which we certainly get <span class="math inline"><em>r</em><em>a</em><em>n</em><em>d</em><em>o</em><em>m</em>()%1 = 0</span>, so <span class="math inline"><em>a</em><em>n</em><em>s</em> = 2</span>. Expected value of <span class="math inline"><em>a</em><em>n</em><em>s</em></span> is therefore <span class="math inline">1 × 1/2 + 2 × 1/2 = 1.5</span>.</em></p>