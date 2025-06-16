<p>Dolan has a stack of card. Each card is numbered from 1 to n from top to bottom. His nephews want to play with the cards. Each nephew can only do one kind of operation.</p>
<p>Nephew number 1 will reverse the order of the card from i-th to j-th position.</p>
<p>Nephew number 2 will ask uncle Dolan what is the card number on i-th position.</p>
<p>Nephew number 3 will ask uncle Dolan in what position is the card number i.</p>
<p>Since Dolan is a good uncle, he will have to answer all questions correctly. Please help Dolan.</p>
<h3>Input</h3>
<p>First line on input is n and q, the number of cards (n&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;100000)&nbsp;and number of operations by the nephews (q&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;100000). The next q lines will contain the operation by the nephews.&nbsp;</p>
<p>For each operation, the first number will be the nephew number. The second (and possibly third) number is i (and j) from the description above (1&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;i <span style="text-decoration: underline;">&lt;</span> j&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;n).</p>
<h3>Output</h3>
<p>For each question asked by the nephews (operation 2 and 3), output a single line containing the answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 5<br>1 2 6<br>2 5<br>1 4 9<br>3 4<br>2 4&nbsp;</pre>
<pre><strong>Output:</strong>
3<br>9<br>9&nbsp;</pre>
<p><strong> Input file is huge, use faster I/O (scanf for C)</strong></p>