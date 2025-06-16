<p>One of the simplest sorting algorithms, the Bubble Sort, can be expressed as (0-based array):</p>
<p><span style="font-family: 'courier new', courier;">procedure bubbleSort( A : list of sortable items )&nbsp;&nbsp;</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp; n = length(A)</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp; repeat</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; swapped = false</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for i = 1 to n-1 inclusive do</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /* if this pair is out of order */</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if A[i-1] &gt; A[i] then</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /* swap them and remember something changed */</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; swap( A[i-1], A[i] )</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; swapped = true</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end if</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; end for</span></p>
<p><span style="font-family: 'courier new', courier;">&nbsp;&nbsp; &nbsp; until not swapped</span></p>
<p><span style="font-family: 'courier new', courier;">end procedure</span></p>
<p>Now, given an array of N integers, you have to find out how many swap opeartions occur if the Bubble Sort algorithm is used to sort the array.</p>
<h3>Input</h3>
<p>Input begins with a line containing an integer <strong>T(1&lt;=T&lt;=100)</strong>, denoting the number of test cases. Then T test cases follow. Each test case begins with a line containing an integer <strong>N(1&lt;=N&lt;=10000)</strong>, denoting the number of integers in the array, followed by a line containing <strong>N</strong> space separated 32-bit integers.</p>
<h3>Output</h3>
<p>For each test case, output a single line in the format <strong>Case X: Y</strong>, where <strong>X</strong> denotes the test case number and <strong>Y</strong> denotes the number of swap operations needed modulo 10000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
4
3 2 1 4

<strong>Output:</strong>
Case 1: 3
</pre>