<p>Computing the determinant of a matrix using Gaussian elimination takes O(n^3). &nbsp;On the other hand, computing the determinant of tridiagonal matrix is O(n) using a recurrence. &nbsp;In this problem you will compute the determinant of banded matrices. &nbsp;A band matrix is a sparse matrix, whose non-zero entries are confined to a diagonal band, comprising the main diagonal and zero or more diagonals on either side. &nbsp;In this problem, given a banded <strong>NxN </strong>square integer matrix with <strong>M</strong> bands on each side of the diagonal, we ask you to compute the determinant of this matrix. &nbsp;For example a tridiagonal matrix has exactly 1 band on each side, and the 8x8 Matrix in the sample input has 2 bands on each side. &nbsp;For a good discussion of banded matrices, see Thorson's paper at:</p>
<p>http://sepwww.stanford.edu/oldreports/sep20/20_11_abs.html</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>A total of &lt;10 inputs. &nbsp;For each input,</p>
<p>First line has dimension, <strong>N (1&lt;N&lt;501)</strong>, of the matrix, followed by <strong>N</strong> lines with <strong>N</strong> integers, each less than <strong>10001</strong>, and greater than <strong>-10001</strong>. &nbsp;It is guarantteed that the number of bands on each side of the diagonal, <strong>M &lt; 51. &nbsp;</strong>That is there are at most <strong>101 </strong>bands in total including the diagonal. &nbsp;Use scanf IO, and avoid stl IO.</p>
<h3>Output</h3>
<p>For each input matrix, output its determinant <strong>modulo 10^9+7.</strong></p>
<p><em>Hint:</em> Use Montgomery multiplication for fast computation, i.e., see:<br>http://everything2.com/title/Montgomery%2520multiplication</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong><strong><br></strong><strong>2<br>2 0<br>0 2<br></strong><strong>2<br>1 0<br>0 1<br>8<br>1 0 -1 0 0 0 0 0<br>-1 1 0 -1 0 0 0 0<br>-1 0 -1 1 -1 0 0 0<br>0 -1 0 -1 0 -1 0 0<br>0 0 -1 0 1 0 -1 0<br>0 0 0 -1 -1 1 0 -1<br>0 0 0 0 -1 0 -1 1<br>0 0 0 0 0 -1 0 -1<br></strong><strong><br>Output:<br>4<br>1<br>36<br><br></strong>

</pre>