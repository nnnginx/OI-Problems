<p>Nancy and Pranjali are best friends. For her birthday, Pranjali bought a beautiful bracelet for Nancy, made of ��N�� multi-coloured pearls. Although stunned by the beauty of the pearls and touched by the gesture, Nancy felt that the arrangement of pearls could be changed somewhat, to make the bracelet even more beautiful. After thinking for a long time and making complex calculations, she came up with a formula to calculate the Elegance Factor (E) of the bracelet.</p>
<p>Starting from a particular pearl, she numbers all the pearls from 0 to N-1. Next, she assigns a numeric value to each distinct colour of the pearls, based on RGB values. Thus the bracelet can be represented by a circular integer array ��A�� of size N. Also she comes up with another array, ��B�� also of size N. Now, the Elegance Factor is given by:</p>
<p>E = sum (i = 1 to n-1) {(A [i] �C A [i-1]) * B[i]}</p>
<p>Obviously, Nancy wants to find an arrangement with the maximum value of E. If there are multiple such arrangements, then she wants the lexicographically smallest one.</p>
<p>Once she has found the required arrangement, Nancy proceeds to re-arrange the pearls in the bracelet. However, Pranjali does not like the fact that her friend is making so many changes to her gift. To make her task much harder, she gives Nancy a number, D, and tells her that in 1 move, she can interchange the positions of 2 pearls only if they are at a distance D from each other.</p>
<p>Nancy does not want to upset her friend, but she also wants to finish the rearrangement as fast as possible. Can you help her find the minimum number of moves to finish the re-arrangement? If it is not possible to reach the desired arrangement, output -1.</p>
<p>&nbsp;</p>
<p>Note 1: In case of multiple possible arrangements with the maximum elegance factor, the desired one is always the lexicographically smallest one, irrespective of whether it can be reached or not.</p>
<p>Note 2: &nbsp;There can be at most 3 distinct colours of the pearls in the bracelet</p>
<p>Note 3: Remember, the bracelet is circular. The distance D can be in both directions.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases.</p>
<p>First line of each test case contains 2 space separated integers, N and D.</p>
<p>The next line contains N space separated integers representing array A.</p>
<p>The next line contains N space separated integers representing array B.</p>
<h3>Output</h3>
<p>Output a single integer, the minimum number of moves, or -1 if not possible.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>5 1</p><p>2 3 4 2 3</p><p>0 0 0 0 0</p><strong>Output:</strong>
3</pre>
<pre><strong>Explanation:</strong></pre>
<pre><p>For all arrangements, E = 0. Therefore the desired arrangement is the lexicographically&nbsp;</p><p>smallest one i.e. 2 2 3 3 4.</p><p>The 3 pairs of indices to be exchanged (in order) to achieve this are (0 based indexing):</p><p>(i) 2-3;</p><p>(ii) 3-4;</p><p>(iii) 1-2; </p><p>&nbsp;</p><p><strong>Constraints:</strong></p><p>1 &lt;= T &lt;= 5</p><p>2 &lt;= N &lt;= 14</p><p>1 &lt;= D &lt;= N-1</p><p>1 &lt;= A[i] &lt;= 1000000</p><p>0 &lt;= B[i] &lt;= 1000000</p></pre>