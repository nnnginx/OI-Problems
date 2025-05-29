<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Biologists have discovered a strange DNA molecule, best described as a sequence of N characters from&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the set {A, B}. An unlikely sequence of mutations has resulted in a DNA strand consisting only of A‟s.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Biologists found that very odd, so they began studying the mutations in greater detail.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">They discovered two types of mutations. One type results in changing a single character of the&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">sequence (A → B or B → A). The second type changes a whole prefix of the sequence, specifically&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">replacing all characters in positions from 1 to K (for some K between 1 and N, inclusive) with the other&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">character (A with B, B with A).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Compute the least possible number of mutations that could convert the starting molecule to its end&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">state (containing only A characters). Mutations can occur in any order</div>
<p>&nbsp;</p>
<p>Biologists have discovered a strange DNA molecule, best described as a sequence of N characters from&nbsp;</p>
<p>the set {A, B}. An unlikely sequence of mutations has resulted in a DNA strand consisting only of A's.&nbsp;</p>
<p>Biologists found that very odd, so they began studying the mutations in greater detail.</p>
<p>They discovered two types of mutations. One type results in changing a single character of the&nbsp;</p>
<p>sequence (A → B or B → A). The second type changes a whole prefix of the sequence, specifically&nbsp;</p>
<p>replacing all characters in positions from 1 to K (for some K between 1 and N, inclusive) with the other&nbsp;</p>
<p>character (A with B, B with A).</p>
<p>Compute the least possible number of mutations that could convert the starting molecule to its end&nbsp;</p>
<p>state (containing only A characters). Mutations can occur in any order</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input contains the positive integer N (1 ≤ N ≤ 1 000 000), the length of the molecule.</p>
<p>The second line of input contains a string with N characters, with each character being either A or B.&nbsp;</p>
<p>This string represents the starting state of the molecule.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The first and only line of output must contain the required minimum number of mutations.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
4
ABBA

<strong>Output 1:</strong>
2</pre>
<pre><strong>Input 2:</strong>
5
BBABB

<strong>Output 2:</strong>
2
</pre>
<pre><strong>Input 3:</strong>
12
AAABBBAAABBB

<strong>Output 3:</strong>
4</pre>