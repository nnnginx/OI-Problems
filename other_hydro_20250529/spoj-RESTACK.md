<p>Farmer John has just ordered a large number of bales of hay.  He would like<br>to organize these into N piles (1 &lt;= N &lt;= 100,000) arranged in a circle,<br>where pile i contains B_i bales of hay.  Unfortunately, the truck driver<br>delivering the hay was not listening carefully when Farmer John provided<br>this information, and only remembered to leave the hay in N piles arranged<br>in a circle.  After delivery, Farmer John notes that pile i contains A_i<br>bales of hay.  Of course, the A_i's and the B_i's have the same sum.</p>
<p>Farmer John would like to move the bales of hay from their current<br>configuration (described by the A_i's) into his desired target<br>configuration (described by the B_i's).  It takes him x units of work to<br>move one hay bale from one pile to a pile that is x steps away around the<br>circle.  Please help him compute the minimum amount of work he will need to<br>spend.</p>
<h3>Input</h3>
<p>* Line 1: The single integer N.</p>
<p>* Lines 2..1+N: Line i+1 contains the two integers A_i and B_i (1 &lt;=<br> A_i, B_i &lt;= 1000).</p>
<p>Example:</p>
<p>4<br>7 1<br>3 4<br>9 2<br>1 13</p>
<h3>OUTPUT:</h3>
<p>A single line containing one number,answer to the problem.</p>
<p>Example:</p>
<p>13</p>