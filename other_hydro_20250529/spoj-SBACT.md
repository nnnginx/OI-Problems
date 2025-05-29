<!-- Block added 2009-04-02 SRL --> <!-- End block -->
<p>&nbsp;</p>
<p>&nbsp;Given an nxn grid of cells, a bacteria colony can colonize these cells. Their growth after every second is governed by the following rules:</p>
<p>1) One new bacteria is born in cell (i ,j) if and only if either one of its four neighboring cells or the cell(i,j) itself has a bacteria population more than or equal to the threshold value, k.</p>
<p>2) Already living bacterias do not die.</p>
<p>Given, the initial state of the nxn cell grid, you need to accurately estimate the time by when the total bacteria population reaches m.</p>
<h3>Input</h3>
<p>First line contains t, number of test cases.</p>
<p>Each test case starts with n (side length of grid) , k (growth threshold) and m (final population).</p>
<p>Next n lines contain an nxn grid of integers, where ith row,jth column has an integer representing the number of bacteria's present initially at cell(i,j).</p>
<p>1&lt;  n &lt;= 100 , 0&lt;  k &lt;= 2^45 , 0&lt; m &lt;= 2^45,</p>
<p>There are no more than n cells with initial population equal to or greater than k.</p>
<h3>Output</h3>
<p>For each test case print the number of seconds required for the total bacteria population to reach m. If m can never be reached print "Not possible" (quotes for clarity).</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><pre>1<br>3 5 15<br>0 0 0<br>0 3 0<br>0 0 5<br><br><br></pre>
<br><br><strong>Output:</strong><br>
<pre>3<br><br></pre>
<br></pre>