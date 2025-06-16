<p style="text-align: right;">“<em>It’s Black, It’s White, It’s Tough For You To Get By</em>”<br>Michael Jackson (1958-2009)</p>
<p><br>You have a sequence of integers. You can paint each of the integers black or white, or leave<br>it unpainted. The black integers must appear in ascending order and the white integers<br>must appear in descending order. The ascending/descending order must be strict, that<br>is, two integers painted with the same color cannot be equal. Paint the sequence so as to<br>minimize the number of unpainted integers.</p>
<h3>Input</h3>
<p>The input contains several test cases, each one described in exactly two lines. The first line<br>contains an integer N indicating the number of elements in the sequence (1 ≤ N ≤ 200).<br>The second line contains N integers Xi separated by single spaces, representing the<br>sequence to paint (1 ≤ Xi ≤ 10<sup>6</sup> for 1 ≤ i ≤ N ). The last line of the input contains a<br>single −1 and should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case output a single line with an integer representing the minimum number<br>of unpainted elements of the sequence, when the sequence is painted optimally following<br>the rules described above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>8<br>1 4 2 3 3 2 4 1<br>12<br>7 8 1 2 4 6 3 5 2 1 8 7<br>-1<br><br><strong>Output:</strong>
0<br>2</pre>