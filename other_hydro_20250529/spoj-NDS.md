<p>Subham and Dewang both are playing with numbers. Subham gives Dewang an array of numbers and asks him to tell the minimum possible last number of a increasing sequence of length&nbsp;<strong>L</strong>.</p>
<p><strong>Note: </strong>Check the sample I/O for more clarity.</p>
<h3>Input</h3>
<p>Input consists of number of test cases&nbsp;<strong>T</strong>. Each test case contains size of array i.e <strong>N</strong>. Next line contains&nbsp;<strong>N</strong> space separated elements of array.  Next line contains length of the increasing sequence i.e.&nbsp;<strong>L</strong>.</p>
<h3>Constraignts</h3>
<p>1 ¡Ü T ¡Ü 100<br>0 ¡Ü N ¡Ü 10<sup>6</sup><br> 0 ¡Ü a[i] ¡Ü 10<sup>6</sup></p>
<h3>Output</h3>
<p>You have to print the minimum possible last number of a sequence and if their is no increasing sequence of length&nbsp;<strong>L</strong>, then print "-1" without the quotes.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
7
9 7 2 5 4 11 12 
3

<strong>Output:</strong>
11</pre>
<h3>Explanation</h3>
<p>In sample input, possible increasing sequences of length  L = 3 are  (9, 11, 12), (7, 11, 12), (2, 5, 11), (2, 4, 11), (2, 5, 12), (2, 4, 12), (2, 11, 12), (5, 11, 12), (4, 11, 12) and the minimum last number is 11 for the sequences  (2, 5, 11) and (2, 4, 11). Hence, the answer is 11.</p>
<p>&nbsp;</p>