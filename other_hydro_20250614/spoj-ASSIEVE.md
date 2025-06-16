<p>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.css" integrity="sha384-zB1R0rpPzHqg7Kpt0Aljp8JPLqbXI3bhnPWROx27a9N0Ll6ZP/+DiW/UqRcLbRjq" crossorigin="anonymous">
<script defer="" src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/katex.min.js" integrity="sha384-y23I5Q6l+B6vatafAwxRu/0oK/79VlbSz7Q9aiSZUvyWYIYsd+qj+o24G5ZU2zJz" crossorigin="anonymous"></script>
<script defer="" src="https://cdn.jsdelivr.net/npm/katex@0.11.1/dist/contrib/auto-render.min.js" integrity="sha384-kWPLUVMOks5AQFrykwIup5lo0m3iMkkHrD0uJ4H5cjeGihAutqP0yW0J6dpFiVkI" crossorigin="anonymous" onload="renderMathInElement(document.body);"></script>

</p>
<p>You are given a commutative associative unitary function \(x(i,j)\) defined over all \(0\le i,j,x(i,j)\lt 4\). In other words, this function satisfies, for all \(0\le i, j, k \lt 4\):</p>
<ol>
<li>\(x(i,j)=x(j,i)\)</li>
<li>\(x(x(i, j), k)=x(i, x(j, k))\)</li>
<li>\(x(0, i)=i\)</li>
</ol>
<p>Define a function \(f(n)\) for all positive integers \(n\) such that:</p>
<ol>
<li>\(f(p^k)=(pk)\bmod 4\), that is, the remainder when \(pk\) is divided by 4</li>
<li>If \(\gcd(a, b)=1\), then \(f(ab)=x(f(a),f (b))\)</li>
</ol>
<p>Define:</p>
<p>$$g(n,k,r)=\sum_{i=1}^ni^k[f(i)=r]$$</p>
<p>where \([f(i)=r]\) is the <a href="http://mathworld.wolfram.com/IversonBracket.html">Iverson bracket</a>.</p>
<p>Given the function \(x\) and two integers \(m\), \(k\), for all integers \(1\le i\le\lfloor\sqrt n\rfloor\), calculate \(g(\lfloor\frac ni\rfloor, k, 0...3)\) modulo \(998\ 244\ 353\).</p>
<h3>Input</h3>
<p>The first line contains two integers \(m\) and \(k\). (\(1\le m\le 10^{10}\), \(0 \le k \le 1000\))</p>
<p>The following 4 lines contains 4 integers each. The i-th row j-th integer contains \(x(i-1,j-1)\).</p>
<h3>Output</h3>
<p>Output \(\lfloor\sqrt n\rfloor\) lines containing 4 integers each. The i-th row j-th integer contains \(g(\lfloor\frac ni\rfloor, k, j-1)\) modulo \(998244353\).</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre style="font-family: monospace; font-size: 0.875em; margin: 0.5em 0px; padding: 0.3em 0.5em; border: 1px solid #dddddd; background: #f8f8f8; border-radius: 3px; overflow: auto; color: rgba(0, 0, 0, 0.75);">10 0
0 1 2 3
1 2 3 0
2 3 0 1
3 0 1 2</pre>
<p><strong>Output:</strong></p>
<pre style="font-family: monospace; font-size: 0.875em; margin: 0.5em 0px; padding: 0.3em 0.5em; border: 1px solid #dddddd; background: #f8f8f8; border-radius: 3px; overflow: auto; color: rgba(0, 0, 0, 0.75);">2 2 3 3
2 1 1 1
1 0 1 1</pre>
<p><strong>Input:</strong></p>
<pre style="font-family: monospace; font-size: 0.875em; margin: 0.5em 0px; padding: 0.3em 0.5em; border: 1px solid #dddddd; background: #f8f8f8; border-radius: 3px; overflow: auto; color: rgba(0, 0, 0, 0.75);">100 100
0 1 2 3
1 0 3 2
2 3 0 1
3 2 1 0</pre>
<p><strong>Output:</strong></p>
<pre style="font-family: monospace; font-size: 0.875em; margin: 0.5em 0px; padding: 0.3em 0.5em; border: 1px solid #dddddd; background: #f8f8f8; border-radius: 3px; overflow: auto; color: rgba(0, 0, 0, 0.75);">457599333 476580683 403589597 762762658
361221912 612412943 661908092 483645330
242804711 682542199 535167020 465246643
913280460 516845083 917292729 390364642
39265044 919790719 181416471 421087779
530140662 31014314 181416471 226287885
982924733 31014314 851084249 226287885
982924733 938693280 851084249 226287885
982924733 938693280 851084249 435036575
982924733 938693280 851084249 138976409</pre>