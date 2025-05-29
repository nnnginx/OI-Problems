<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given two grids of characters , consists of characters from 'a' to 'z' only. we name two grids 'A' and 'B'.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now , we need to find the lexicographically largest triplet &lt;i,j,k&gt;&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given that :&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">f(A,i,j,k)=B , 0&lt;=j&lt;k&lt;n and 1&lt;=i&lt;=n-2 (where 'n*n' is the size of grid)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(i.e. function 'f' operated on matrix 'A' with 'i' , 'j' and 'k' parametrs gives matrix 'B'.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Description of function 'f' :&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">f(M,i,j,k) : function operated on matrix 'M' does following operations in the given order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1) Take rows from index '0' to 'i' of the given grid M and flip it, i.e.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for( each column Ci ) reverse(A[0..i][Ci])</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2) Take colums from index '0' to 'j' of the grid and flip it, i.e.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for( each row Ri ) reverse(A[Ri][0..j])</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3) Take colums from index 'k' to 'n-1' of the grid and flip it, i.e.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for( each row Rj ) reverse(A[Rj][k...n-1]</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4) Remove columns indexed '0' to 'j' and concatenate on the right of the grid in the same order, making new grid.</div>
<p>Given two grids of characters , consists of characters from 'a' to 'z' only. we name two grids 'A' and 'B'.</p>
<p>Now , we need to find the lexicographically largest triplet &lt;i,j,k&gt; &nbsp; ( Assuming that one such solution does always exists )</p>
<p><strong>Given that :</strong>&nbsp;</p>
<p>f(A,i,j,k)=B , 0&lt;=j&lt;k&lt;n and 1&lt;=i&lt;=n-2 (where 'n*n' is the size of grids)</p>
<p>(i.e. function 'f' operated on matrix 'A' with 'i' , 'j' and 'k' parametrs gives matrix 'B'.</p>
<p>&nbsp;</p>
<p>Description of function 'f' :&nbsp;</p>
<p>f(M,i,j,k) : function operated on matrix 'M' does following operations in the given order.</p>
<p>&nbsp;</p>
<p>1) Take rows from index '0' to 'i' of the given grid M and flip it, i.e.</p>
<p>for( each column Ci ) reverse(A[0..i][Ci])</p>
<p>&nbsp;</p>
<p>2) Take colums from index '0' to 'j' of the grid and flip it, i.e.&nbsp;</p>
<p>for( each row Ri ) reverse(A[Ri][0..j])</p>
<p>&nbsp;</p>
<p>3) Take colums from index 'k' to 'n-1' of the grid and flip it, i.e.</p>
<p>for( each row Rj ) reverse(A[Rj][k...n-1]</p>
<p>&nbsp;</p>
<p>4) Remove columns indexed '0' to 'j' and concatenate on the right of the grid in the same order, making new grid.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line contains one integer 'n' (n*n is size of grid)</p>
<p>Following n lines (i.e. line numbers 2 to n+1 ) containes strings each of size 'n' for grid 'A'.</p>
<p>Following n lines (i.e. line numbers n+2 to 2n+1) containes strings each of size 'n' for grid 'B'.</p>
<h3 style="text-align: left;"><strong>Constraints:</strong></h3>
<h3 style="text-align: left;"><span style="font-size: 12px; font-weight: normal;">1) 5&lt;=n&lt;=1000&nbsp;</span></h3>
<h3 style="text-align: left;"><span style="font-size: 12px; font-weight: normal;">2) String contains only lower case alphabets</span></h3>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Three integers (space separated) in one line representing i , j and k respectively (lexicographically largest solution).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
ooscz
hkaea
nnzth
khdlf
rejtf
fldhk
htznn
aeakh
zcsoo
ftjer

<strong>Output:</strong>
3 3 4<span style="white-space: normal;">
</span></pre>