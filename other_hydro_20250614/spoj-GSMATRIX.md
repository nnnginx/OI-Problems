<p>Mr. Ganesh, a friend of Mr. Dengklek, give Mr. Dengklek a big matrix A dan asking the result of A^N. Because the matrix A is too big and Mr Dengklek doesn't have a lot of time, he wants to minimize the number of multiplication needed for computing A^N. In this case, assume Mr. Dengklek always stores the matrices that Mr. Dengklek ever computed, thus, if anytime Mr. Dengklek wants to use that matrix again, he can just directly use it without recomputing it.</p>
<p>You must help Mr. Dengklek to find out the minimum number of multiplication required to compute A^N.</p>
<h3>Input</h3>
<p>The first line consist of a single integer N (1 ¡Ü N ¡Ü 120).</p>
<h3>Output</h3>
<p>In the first line, output the result asked in the problem statement above.</p>
<h3>Example Explanation</h3>
<p>Here is one of the possible minimum calculation to get A^15.</p>
<p>Matrices that Mr. Dengklek have : A</p>
<p>1st multiplication : A * A = A^2</p>
<p>Matrices that Mr. Dengklek have : A, A^2</p>
<p>2nd multiplication : A*A^2 = A^3</p>
<p>Matrices that Mr. Dengklek have : A, A^2, A^3</p>
<p>3rd multiplication : A^3*A^3 = A^6</p>
<p>Matrices that Mr. Dengklek have : A, A^2, A^3, A^6</p>
<p>4th multiplication : A^6*A^6 = A^12</p>
<p>Matrices that Mr. Dengklek have : A, A^2, A^3, A^6,A^12</p>
<p>5th multiplication : A^12*A^3 = A^15</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
15

<strong>Output:</strong>
5
</pre>