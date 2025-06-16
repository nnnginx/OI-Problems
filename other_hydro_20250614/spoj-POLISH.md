<p>Russell can't wait to know Poland. As he waits he decided to learn a little of the Polish Language. To do this in a funny way he intends to use an old Polish dictionary and play a game he learned from the old Carl.</p>
<p>Given a word s in the dictionary, Russell is interested in sequences of suffixes of s. But not just any one! Russell considers amusing sequences of suffixes with the following properties:</p>
<ul>
<li>The suffixes appear in increasing sizes.</li>
<li>The suffixes appear in lexicographic order.</li>
</ul>
<p>As an example, if s = ABACA then the sequences (ABACA), (A, CA) and (A, ACA, BACA) please Russell but (ABACA, ACA) or (CA, ACA) doesn't.</p>
<p>Help Russell find the number of amusing sequences of suffixes of a given word s modulo 1000000007 (10^9 + 7).</p>
<h3>Input</h3>
<p>The input consists of several test cases. Each test case consists of only one line containing a string <strong>S</strong> with 1 to 100000 (10^5) uppercase latin letters (A - Z).</p>
<h3>Output</h3>
<p>For each test case output a single line containing the number of amusing sequences of suffixes of <strong>S</strong> modulo 1000000007 (10^9 + 7).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
ABACA<br>NIE<br>PIJ<br>WODY<br>CAMPINAS

<strong>Output:</strong>
11<br>7<br>5<br>8<br>20
</pre>