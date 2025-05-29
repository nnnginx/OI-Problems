<p>Apoorv has an array of n integers.Inversion count of an array is defined by number of pair of indices(i,j)  such that i&lt;j  and arr[i]&gt;arr[j] .You are given an integer p.Apoorv has to find the subarray with maximum inversion count among all subarrays of size p.Apoorv find this job very tough so he turns to you for help.</p>
<p>Constraints :</p>
<p>1&lt;=n&lt;=500000</p>
<p>-1000000000&lt;=arr[i]&lt;=1000000000</p>
<p>1&lt;=p&lt;=n</p>
<h3>Input</h3>
<p>First line contains two integers n and p.</p>
<p>Next line contains n space separated integers denoting the elements of the array.</p>
<h3>Output</h3>
<p>Output two space separated integers first integer should be the<strong> starting index</strong> (1-based indexing) of the subarray and next integer would be the <strong>count of inversions in that subarray</strong>.In case there is a tie in maximum inversion count&nbsp; print the <strong>smallest</strong> starting index among the subarrays having maximum inversion count.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span>10 5</span>
<span>15 51 44 44 76 50 29 88 48 50</span>
<strong>Output:</strong>
5 6
</pre>