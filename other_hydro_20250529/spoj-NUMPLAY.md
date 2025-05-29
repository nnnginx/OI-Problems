<p>consider a set of 4 numbers {1,3,5,7} .. Form a number using these digits in the set under the following constraints ,1 can be followed only by 3((i.e) the number may contain 13 but not 15 or 17 or 11 eg:13573 is valid but not 113573), 3 can be followed only by 1 and 5, 5 can be followed only by 7 ,7 can be followed only by 5 and 3</p>
<p>Find the number of such numbers of length n</p>
<p>eg:</p>
<p>37,51,53,71 are all not a valid number of length2 ,131 is a valid number of length 3,1357,1313 are all a valid number of length 4 but 11 or 1537 or15 or 17 or 33 is not a valid number..</p>
<h3>Input</h3>
<p>t, First line of input contains number of test cases 0&lt;=t&lt;=40</p>
<p>remaining t lines consist of length n for each test case 0&lt;=n&lt;=10000</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Output the number of possible numbers of length n followed by a line(note long long int &nbsp;in c++ may not be sufficient)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>2</pre>
<pre>1</pre>
<pre>4

<strong>Output:</strong></pre>
<pre>6</pre>
<pre>4</pre>
<pre>13</pre>
<pre>Note : time limit is reduced for checking the accuracy</pre>