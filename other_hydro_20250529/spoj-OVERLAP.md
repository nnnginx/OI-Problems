<p>A large package of chocolate has arrived to the kindergarten. Each child has received one chocolate. To teach the children to share, the teachers have decided that each child will share her/his chocolate with others.</p>
<p>The children are given a crossword puzzle filled by M x M characters. Each child has to find a word (any word) in the crossword. After each child found a word, the chocolates are shared as follows: each child will share her/his chocolate with the children whose words overlap with her/his word in at least one common field.</p>
<p>Write a program that, for given positions of the words that the children have found in the crossword, for each child prints the number of children with whom she/he will share her/his chocolate.</p>
<p><span style="font-size: 1.17em;"><strong>Input</strong></span></p>
<p>The first line contains an integer N (1 ¡Ü&nbsp;N ¡Ü&nbsp;300 000), the number of children.</p>
<p>The second line contains an integer M (1 ¡Ü&nbsp;M ¡Ü&nbsp;100 000), dimensions of the crossword puzzle.</p>
<p>Each of the following N lines contains four integers R1, S1, R2, S2 from the interval [1, M]. They indicate that the word of the child is on the successive fields from (R1, S1) to (R2, S2), including these fields. These fields will always be in the same row or the same column. Moreover, (R1 = R2 and S1 &lt; S2) or (S1 = S2 and R1 &lt; R2) will hold.</p>
<p><span style="font-size: 1.17em;"><strong>Output</strong></span></p>
<p>Print the required N numbers, where K-th number corresponds to the K-th child in the input.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
5
4
2 1 2 4
2 1 2 4
4 1 4 3
1 3 3 3
2 3 4 3
<strong><br></strong></pre>
<pre><strong>Output:</strong>
3
3
1
3
4
</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
5
10
2 4 9 4
2 7 9 7
6 7 8 7
4 2 4 9
7 2 7 9
<strong><br></strong></pre>
<pre><strong>Output:</strong>
2
3
2
2
3
</pre>