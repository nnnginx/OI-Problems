Given an NxN matrix of characters. We start at position (1,1) and want to reach (N,N) in exactly 2N-1 moves. Each move consists of movement in one of the four standard directions. As we move, we collect the characters found in our positions forming a string. We now constrain our attention to all paths that do not cross the diagonal of
the matrix. However the parts of the path can be on the diagonal line. These paths can be classified into two partitions; the paths that lie above and paths that lie below the diagonal. Each path is represented by a string of characters formed by the ordered concatenation of
characters found on the way. If we consider the set of all valid paths, (both upper and lower) get their corresponding strings, sort them all in alphabetical order, we obtain the (ordered) master set. Note that
the master set might contain duplicates, and all strings in the master set consist of exactly 2N-1 characters. Let M be the total number of strings in the master set, given an integer I, we need to find the string with index = I (modulo M) within the master set.<br>
  If Master Set = { ¡°A¡±,¡±B¡±,¡±B¡±,¡±C¡± } (although this set can never be a master set!)<br>
  I=0 produces ¡°A¡±, while I=2 and I=5, produces ¡°B¡±.<p></p>
<p><strong>Constraints: </strong><br>
  N&lt;=30.<br>
  I&lt;=10<sup>18</sup>. ¡®I¡¯ will fit into a 64-bit integer.</p>

<h3>Input</h3>
<p>  T-number of test cases<br>
  N I<br>
  Next is the NxN matrix of characters, N characters per line.<br>
  All characters are between ¡®A¡¯-¡®Z¡¯ (only uppercase).</p>

<h3>Output</h3>
<p>For each test case output the corresponding string sought for in the master set.</p>

<h3>Example</h3>
<tt>
<p><strong>Sample Input:</strong><br>
  2 <br>
  3 18<br>
  DAA<br>
  BDA<br>
  BBD <br>

  3 18<br>
  DAA<br>
  ADA<br>
  AAD</p>
<p><strong>Sample Output:</strong><br>
  DBBBD<br>

  DADAD</p>
</tt>
<p><strong>Explanation: </strong><br>
  Test case I: Master Set = { ¡°DAAAD¡±, ¡°DADAD¡±,¡±DBBBD¡±,¡±DBDBD¡±}<br>
  Test case II: Master Set = { ¡°DAAAD¡±,¡±DAAAD¡±,¡±DADAD¡±,¡±DADAD¡±}<br>
</p>