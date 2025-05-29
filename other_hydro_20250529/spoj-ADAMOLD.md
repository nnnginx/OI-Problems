<p>As you might already know, Ada the Ladybug is a farmer. She has a long furrow in which she grows vegetable (while each vegetable is indentified by a bloom-value). The more vegetable is in the furrow the bigger risk of mold there is. More specificaly the mold-value can be obtained as sum of <strong>xor</strong> of all pairs of vegetable's bloom-values.</p>
<p>Ada has bought a few wooden separators which could possibly reduce the mold-value. It works in following manner: she can put the separators between some plants, dividing the furrow into multiple segments. The mold-value will then becomes the sum of mold-values of all the segments (independently). Can you find the minimal possible mold-value?</p>
<h3>Input</h3>
<p>The first line of input containts two integers <strong>N, K</strong>:  <strong> 1 ¡Ü K &lt; N ¡Ü     5000</strong>, the length of furrows and the number of separators.</p>
<p>The next lines will contain <strong>N</strong> numbers <strong>0 ¡Ü A<sub>i</sub> ¡Ü     10<sup>9</sup></strong>, the bloom-values of vegetable.</p>
<h3>Output</h3>
<p>Output the minimal possible mold-value.</p>
<h3>Example Input</h3>
<pre>6 1
1 2 3 4 5 6
</pre>
<h3>Example Output</h3>
<pre>12
</pre>
<h3>Example Input 1</h3>
<pre>4 3
5 3 5 3
</pre>
<h3>Example Output 1</h3>
<pre>0
</pre>
<h3>Example Input 2</h3>
<pre>7 2
5 3 5 3 5 3 4
</pre>
<h3>Example Output21</h3>
<pre>24
</pre>
<h3>Example Input 3</h3>
<pre>9 4
1 2 3 4 5 6 7 666 1024
</pre>
<h3>Example Output 3</h3>
<pre>8
</pre>
<h3>Example Input 4</h3>
<pre>30 8
629470789 417274987 617986533 841737683 297969800 432044389 708142005 156958893 499363651 434034331 176735187 525172817 747109631 949700868 259681519 357968078 818249370 456939952 450487335 529013233 327250536 90354657 643708145 141755216 656041628 661580907 204072850 469709611 834069223 681347499
</pre>
<h3>Example Output 4</h3>
<pre>16154467281
</pre>