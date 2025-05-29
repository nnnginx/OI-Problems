<p>
A straightforward question. Given an array of positive integers you have to print the number of subarrays whose XOR is less than <strong>K</strong>. Subarrays are defined as a sequence of continuous elements <strong>A<sub>i</sub>, A<sub>i+1</sub>, ..., A<sub>j</sub> </strong>. XOR of a subarray is defined as <strong>A<sub>i</sub> ^ A<sub>i+1</sub> ^  ... ^ A<sub>j</sub></strong>. Symbol <strong>^</strong> is Exclusive Or. You can read more about it here:<br> <a href="http://en.wikipedia.org/wiki/Exclusive_or"> http://en.wikipedia.org/wiki/Exclusive_or </a> </p>

<h3>Input Format:</h3>
<p>First line contains<strong> T</strong>, the number of test cases. Each of the test case consists of<strong> N</strong> and <strong>K</strong> in one line, followed by<strong> N</strong> space separated integers in next line. </p>

<h3>Output Format:</h3>
<p>For each test case, print the required answer. </p>

<h3>Constraints:</h3>
<p><strong> 1 ¡Ü T ¡Ü 10<br> 1 ¡Ü N ¡Ü 10^5<br> 1 ¡Ü A[i] ¡Ü 10^5<br> 1 ¡Ü K ¡Ü 10^6<br> Sum of N over all testcases will not exceed 10^5.</strong> </p>

<h3>Sample Input:</h3>
<pre>1
5 2
4 1 3 2 7	</pre>
<h3>Sample Output:</h3>
<pre>3</pre>

<h3>Explanation:</h3>
<p> Only subarrays satisfying the conditions are [1], [1,3,2] and [3,2]. </p>
<p><br> <strong>Problem Setter: Lalit Kundu</strong></p>