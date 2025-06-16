<p>We define a sequence {x}: {x}={x_0, x_1, ¡­ , x_n-1 } where x_i is a interger.</p>
<p>We have a function f: {x}-&gt;{x¡¯} where {x} is a finite sequence.</p>
<p>After we have a finite sequence {x}, we can get f({x}) follow these rules :</p>
<p>&nbsp;</p>
<p>(1). Remove all 0 in x : a 0 b 0 c d 0 e f 0 g =&gt; a b c d e f g</p>
<p>(2). Turn 1 into 100 and -1 into -100 : a 1 b 1 -1 c d e f g =&gt; a 100 b 100 -100 c d e f g</p>
<p>(3). Add all 2^k (k&gt;1) at the end of the sequence : a 2 b 8 c d e 1024 f g =&gt; a 2 b 8 c d e 1024 f g 2 8 1024</p>
<p>(4). Add any positive odd prime x at the end of the sequence x-1 times: a 3 b c 7 d e f 5 g =&gt; a 3 b c 7 d e f 5 g 3 3 7 7 7 7 7 7 5 5 5 5</p>
<p>(5). For any positive composite number (not 2^k, k&gt;1 ), we just keep it once: a 6 b 6 c d 6 e 4 4 f g =&gt; a 6 b c d e 4 4 f g</p>
<p>(6). Keep any t (t&lt;-1) in the sequence.</p>
<p>For a example:</p>
<p>{x}={-5 1 0 2 9 16 7 5 3 2 9 9 -1}</p>
<p>f({x})={-5 100 2 9 16 7 5 3 2 -100 2 2 16 7 7 7 7 7 7 5 5 5 5 3 3}</p>
<p>&nbsp;</p>
<p>We define g({x}) is the sum of all the element in sequence x.</p>
<p>We define h({x}) = g(f({x}))-g({x}).</p>
<p>&nbsp;</p>
<p>A consecutive sequence of x is a sequence {x_i, x_i+1, x_i+2, ¡­ , x_j} where 0&lt;=i&lt;=j&lt;n.</p>
<p>&nbsp;</p>
<p>Now I will give you a sequence {x} .</p>
<p>I want to ask you the maximal h({y}) where {y} is a consecutive sequence of {x}.</p>
<h3>Input</h3>
<p>One line consists one interger N, the length of {x}. &nbsp; (N&lt;=10^5, |x_i|&lt;=10000)</p>
<p>Next N lines, each line consists one interger.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The maximal h({y}) where {y} is a consecutive sequence of {x}. ( |h({y})|&lt;=2^63-1 )</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>5</p><p>1</p><p>2</p><p>6</p><p>6</p><p>3</p><strong>Output:</strong></pre>
<pre><strong>&nbsp;</strong>101
</pre>