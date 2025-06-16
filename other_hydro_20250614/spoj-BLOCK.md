<p>An integer sequence is called <strong>block</strong> iff it is made of two identical and neighboring sequences. For example, (3, 3) and (5, 2, 5, 2) are blocks, while (9, 6, 6, 9) and (1, 1, 1) are not blocks.</p>
<p>An integer sequence is called <strong>non-descreasing</strong> iff its each element (except the last one) is less than or equal to the next one. A sequence containing one or zero elements is also non-decreasing.</p>
<p>You are given an integer sequence and you are to transform it into a <strong>non-decreasing</strong> sequence by multiple using of two types of operations:</p>
<p><strong>Type 1</strong>: removing a block from the sequence (if that block is a consecutive subsequence);</p>
<p><strong>Type 2</strong>: inserting a block into the sequence (so that it becomes a consecutive subsequence).</p>
<p>In all of the test data there will be at least one solution.</p>
<h3>Input</h3>
<p>In the first line there is an integer N (3 �� N �� 40), the size of the given sequence.</p>
<p>In the next line there are N space-separated integers (of size 0 - 100), the elements of the sequence (in order).</p>
<h3>Output</h3>
<p>Output at most 2340 operations.</p>
<p>For each operation, write two or three lines (depending on the type of operation). In the first line write the type of the operation (1 or 2).</p>
<p>If the type of the operation is 1 (removing the block), in the next line write the two numbers: positions in the sequence of the first and the last element of the block you are removing.</p>
<p>If the type of the operation is 2 (adding the block), in the second line write the two numbers: positions in the sequence of the first and the last element of the block after it is added to the sequence. In the next line, write all the elements of the added block (in order). The elements must be integers from the interval [-1000, 1000].</p>
<p>There must be less than 1000 elements in the sequence at any time.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><p>6</p><p>10 20 70 20 70 80</p><br><strong>Output:</strong>
<p>1 </p><p>2 5</p><p>&nbsp;</p><strong>Input:</strong><pre><p>6</p><p>0 4 0 4 4 0</p><p><strong><br></strong></p><p><strong>Output:</strong></p><p>2</p><p>3 4</p><p>4 4</p><p>1</p><p>3 8</p></pre>
</pre>