<p>Consider Pascal’s triangle modulo 2. The first nine rows are given below:</p>
<pre><code>        1 
       1 1 
      1 0 1 
     1 1 1 1 
    1 0 0 0 1 
   1 1 0 0 1 1 
  1 0 1 0 1 0 1 
 1 1 1 1 1 1 1 1 
1 0 0 0 0 0 0 0 1 </code></pre>
<p>Let <span class="math inline"><em>F</em>(<em>n</em>)</span> be the number of <code>1</code> in the first <span class="math inline"><em>n</em></span> rows. So that <span class="math inline"><em>F</em>(0) = 0</span>, <span class="math inline"><em>F</em>(1) = 1</span>, <span class="math inline"><em>F</em>(2) = 3</span>, etc.</p>
<p>Given <span class="math inline"><em>a</em></span>, find the smallest integer <em>n</em> such that <span class="math inline"><em>F</em>(<em>n</em>) ≥ <em>a</em></span>. Let <span class="math inline"><em>N</em>(<em>a</em>)</span> denote this integer.</p>
<h3 id="input">Input</h3>
<p>A list of integers <span class="math inline"><em>a</em><sub>1</sub>, ..., <em>a</em><sub><em>l</em></sub></span>, between <span class="math inline">0</span> and <span class="math inline">10<sup>18</sup></span>, one per line.</p>
<h3 id="output">Output</h3>
<p>The integers <span class="math inline"><em>N</em>(<em>a</em><sub>1</sub>), ..., <em>N</em>(<em>a</em><sub><em>l</em></sub>)</span>, one per line.</p>
<h3 id="example">Example</h3>
<pre><strong>input:</strong>
0
1
4
15

<strong>output:</strong>
0
1
3
6
</pre>