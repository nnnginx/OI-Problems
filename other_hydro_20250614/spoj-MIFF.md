<p>Let p a prime number. A set F<sub>p</sub>={0,1,...,p-1} equipped with the mod p addition and multiplication is a finite field. In this problem you have to compute the multplicative inverse of some F<sub>p</sub> valued (quadratic) matrices.</p>
<p>The input consists of blocks. The structure of a block is:</p>
<p>n p</p>
<p>A<sub>11</sub>...A<sub>1n</sub></p>
<p>...</p>
<p>A<sub>n1</sub>...A<sub>nn</sub></p>
<p>where p is a prime number, 1&lt;n,p&lt;101, and A<sub>ij</sub> are in F<sub>p</sub>. The last block followed by 0 0.</p>
<p>&nbsp;</p>
<p>The ouput for each block is either the multiplicative inverse of a given matrix if it exists or the word "singular"</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><br>4 2<br>1 1 1 1 <br>1 1 0 1 <br>0 0 0 1 <br>0 1 0 1 <br><br>3 7<br>3 5 0 <br>0 5 1 <br>6 6 6 <br><br>2 2<br>1 1 <br>1 0 <br><br>3 5<br>4 0 0 <br>2 4 1 <br>0 2 3 <br><br>3 7<br>0 1 4 <br>6 1 2 <br>2 1 1 <br><br>0 0<br><br><strong>Output:</strong><br><br>0 1 0 1 <br>0 0 1 1 <br>1 1 0 0 <br>0 0 1 0 <br><br>6 3 3 <br>5 1 1 <br>3 3 2 <br><br>0 1 <br>1 1 <br><br>singular<br><br>singular<br></pre>