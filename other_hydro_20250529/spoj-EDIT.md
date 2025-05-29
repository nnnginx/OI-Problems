<p>As any experienced programmer must know the famous problem of "Edit Distance", however this problem is considered an ¡°alternating chain¡± if you have alternately made case sensitive.</p>

<p><b>Example:</b> "AaAaAbB" "B" "a" "aBaCdEf"</p>
<p>Alternating chains are considered in our problem.</p>
<p>We only have one operation that is permitted in exchange for a lower or upper case Latin letter.</p>
<p>Given a string giving the minimum number of changes to be considered an alternating chain.</p>

<h3>Input</h3>
<p>A string with no spaces line containing only uppercase and lowercase letters, one for each line of maximum length 10^3 until end of file</p>

<h3>Output</h3>
<p>For each line print the minimum number of changes to the chain is a "chain alternately"</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
AaAaB
ABaa
a

<strong>Output:</strong>
0
2
0</pre>