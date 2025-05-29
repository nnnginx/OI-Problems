<p><b>"47 is the quintessential random number,"</b> states the 47 society. And there might be a grain of truth in that.</p>

<p>For example, the first ten digits of the Euler's constant are:</p>
<pre>2 7 1 8 2 8 1 8 2 8
</pre>
<p>And what's their sum? Of course, it is 47.</p>

<p>Try walking around with your eyes open. You may be sure that soon you will start discovering occurences of the number 47 everywhere.</p>

<h3>Problem specification</h3>
<p>You are given a sequence <b>S</b> of integers we saw somewhere in the nature. Your task will be to compute how strongly does this sequence support the above claims. </p>

<p>We will call a <b>continuous</b> subsequence of <b>S</b> interesting if the sum of its terms is equal to 47. </p>

<p>E.g., consider the sequence <b>S</b> = (24, 17, 23, 24, 5, 47). Here we have two interesting continuous subsequences: the sequence (23, 24) and the sequence (47). </p>

<p>Given a sequence <b>S</b>, find the count of its interesting subsequences. </p>

<h3>Input specification</h3>
<p>The first line of the input file contains an integer <b>T</b> specifying the number of test cases. Each test case is preceded by a blank line. </p>

<p>The first line of each test case contains the length of a sequence <b>N</b>. The second line contains <b>N</b> space-separated integers : the elements of the sequence. </p>

<h3>Output specification</h3>
<p>For each test case output a single line containing a single integer : the count of interesting subsequences of the given sentence. </p>

<h3>Example</h3>
<pre><b>Input:</b>
2

13
2 7 1 8 2 8 1 8 2 8 4 5 9

7
2 47 10047 47 1047 47 47

<b>Output:</b>
3
4
</pre>
<b>Note: the input file will not exceed 4MB.</b>