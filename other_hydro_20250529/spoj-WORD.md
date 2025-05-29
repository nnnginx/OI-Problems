<p>Ivana made up a long word of N letters. Then she wrote down all K-letter-substrings of that word. For example, if the original word is BANANA and K=3, Ivana writes down the words BAN, ANA, NAN, ANA. The number of these words is, obviously, N-K+1.</p>
<p>Ivana sorted these words in lexicographic&nbsp;order (in the given example, that would be ANA, ANA, BAN, NAN).</p>
<p>But the sad thing happened: Ivana forgot the original word! Your task is to reconstruct it. A unique solution will exist in all of the test data.</p>
<p>Constraints: 3 ¡Ü N ¡Ü 100 000, 2 ¡Ü K ¡Ü 15, K &lt; N.</p>
<h3>Input</h3>
<p>[integers N, K]</p>
<p>[N-K+1 words in lexicographic&nbsp;order, each consisting of capital English letters]</p>
<h3>Output</h3>
<p>[the required word]</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">6 3
ANA
ANA
BAN
NAN</pre>
<strong>Output:</strong></pre>
<pre>BANANA</pre>