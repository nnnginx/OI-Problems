<p><span style="font-size: small;"> Mr. Yagami is playing a game of arrays. He is given two random arrays <strong>A</strong> and <strong>B</strong> consisting of <strong>N</strong> positive integer elements. Game starts by Mr. Yagami assigning <strong>0 or 1</strong> to each element in <strong>A and B</strong>.</span></p>
<p><span style="font-size: small;">After this assignment is done, a graph is constructed with a node for each   element in the array A and B (<strong>2N</strong> nodes) and no edges. The game proceeds with a   valid move being defined in the following way:</span></p>
<ul>
<li>
<p><span style="font-size: small;"> One of the arrays from <strong>A</strong> or <strong>B</strong> is selected.   From the selected array, an element which has been marked <strong>0</strong> is chosen. Let us   call this element as <strong>X</strong>.</span></p>
</li>
<li>
<p><span style="font-size: small;">A set of elements, <strong>Y</strong>, are chosen from the array, which was not chosen in the   first step, such that all elements of <strong>Y</strong> should be marked as <strong>1</strong> and all elements   of <strong>Y</strong> should be greater than <strong>X</strong> and no element of<strong> Y</strong> should be coprime to <strong>X</strong>.</span></p>
</li>
<li>
<p><span style="font-size: small;">Finally an edge is drawn from the node labelled <strong>X</strong> to all the nodes   corresponding to the elements in set <strong>Y</strong>. There can only be a single edge   between any <strong>2</strong> nodes in the graph.</span></p>
</li>
</ul>
<p><span style="font-size: small;"> He can make as many valid moves. Mr. Yagami receives <strong>1</strong> point for each edge   that is drawn in the graph.</span></p>
<p><span style="font-size: small;"> Mr. Yagami is very clever, so he makes the initial assignment in such a way   that it maximizes the number of points he receives in the game. You have to   return the maximum number of points that Mr. Yagami can receive. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> The first line of the input contains a single integer, <strong>N (1 �� N ��   40)</strong><br> The second line of input contains <strong>N</strong> integers separated by a single space   character, which represent the elements of the array <strong>A. (2 �� A[i] ��  10^9)</strong><br> Similarly, the last line of input also contains <strong>N</strong> integers separated by a   single space character, which represent the elements of the array <strong>B. (2 ��    B[i] �� 10^9)</strong></span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> A single integer representing the maximum score which Mr. Yagami can receive. </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">4
16 3 2 9
12 18 13 4</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">8</span></pre>
<h3><span style="font-size: small;">Explanation:</span></h3>
<p><span style="font-size: small;"> He picks 2 from first array. So he gets to put 3 edges ie. 2-&gt;4, 2-&gt;12,   2-&gt;18.<br> Next he picks 3 from the first array. So he gets to put 2 edges ie. 3-&gt;12,   3-&gt;18.<br> Next he picks 9 from the first array. So he gets to put 2 edges ie. 9-&gt;12,   9-&gt;18.<br> Next he picks 16 from the first array. So he gets to put 1 edge ie. 16-&gt;18.   Total edges=8.</span></p>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Lalit Kundu</strong></span></p>