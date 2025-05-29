<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Imagine A is a NxM matrix with two basic properties</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1) Each element in the matrix is distinct and lies in the range of 1&lt;=A[i][j]&lt;=(N*M)</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2) For any two cells of the matrix, (i1,j1) and (i2,j2), if (i1^j1) &gt; (i2^j2) then A[i1][j1] &gt; A[i2][j2] ,where&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 ¡Ü i1,i2 ¡Ü N</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 ¡Ü j1,j2 ¡Ü M.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Given N and M , you have to calculatethe total number of matrices of size N x M which have both the properties</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">mentioned above. &nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Input format:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">First line contains T, the number of test cases. 2*T lines follow with N on the first line and M on the second, representing the number of rows and columns respectively.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Output format:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Output the total number of such matrices of size N x M. Since, this answer can be large, output it modulo 10^9+7</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Constraints:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 ¡Ü N,M,T ¡Ü 1000</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">SAMPLE INPUT&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">SAMPLE OUTPUT&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">4</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Explanation</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">The four possible matrices are:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">[1 3] | [2 3] | [1 4] | [2 4]</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">[4 2] | [4 1] | [3 2] | [3 1]</span></div>
<p><span style="font-size: small;">Imagine A is a NxM matrix with two basic properties</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">1) Each element in the matrix is distinct and lies in the range of 1&lt;=A[i][j]&lt;=(N*M)</span></p>
<p><span style="font-size: small;">2) For any two cells of the matrix, (i1,j1) and (i2,j2), if (i1^j1) &gt; (i2^j2) then A[i1][j1] &gt; A[i2][j2] ,where&nbsp;</span></p>
<p><span style="font-size: small;">1 ¡Ü i1,i2 ¡Ü N</span></p>
<p><span style="font-size: small;">1 ¡Ü j1,j2 ¡Ü M.</span></p>
<p><span style="font-size: small;">^ is Bitwise XOR</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">Given N and M , you have to calculatethe total number of matrices of size N x M which have both the properties</span></p>
<p><span style="font-size: small;">mentioned above. &nbsp;</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Input format:</strong></span></p>
<p><span style="font-size: small;">First line contains T, the number of test cases. 2*T lines follow with N on the first line and M on the second, representing the number of rows and columns respectively.</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Output format:</strong></span></p>
<p><span style="font-size: small;">Output the total number of such matrices of size N x M. Since, this answer can be large, output it modulo 10^9+7</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Constraints:</strong></span></p>
<p><span style="font-size: small;">1 ¡Ü N,M,T ¡Ü 1000</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>SAMPLE INPUT&nbsp;</strong></span></p>
<p><span style="font-size: small;">1</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;"><strong>SAMPLE OUTPUT&nbsp;</strong></span></p>
<p><span style="font-size: small;">4</span></p>
<p><span style="font-size: small;"><strong>Explanation</strong></span></p>
<p><span style="font-size: small;">The four possible matrices are:</span></p>
<p><span style="font-size: small;">[1 3] | [2 3] | [1 4] | [2 4]</span></p>
<p><span style="font-size: small;">[4 2] | [4 1] | [3 2] | [3 1]</span></p>
<p>&nbsp;</p>