<p>Begin a sequence of distinct natural numbers Ni , i = 0, 1, 2,... , with the number B  (= N0) ; generate numbers Ni , i = 1, 2,... , recursively and end the sequence with the last generated number E . The characteristic of numbers and the process for generation are stated below:</p>
<p>
    * Each number in the sequence contains an even number of decimal digits and is of the form f1d1f2d2fk...dk where d1, d2,..., dk , are k distinct digits in increasing order and each fj is a non-zero digit.</p>
<p>    * For i = 0, 1, 2,... , if Ni = f1d1f2d2...fkdk then Ni+1 = F1D1F2D2...FKDK , where K$ \ge$k ; D1, D2,..., DK , are distinct digits that occur in Ni and appear in increasing order in Ni+1 ; and FJ is the frequency of DJ in Ni , for J = 1, 2,..., K . For example if Ni = 102335 then Ni+1 = 1011122315 .</p>
<p>
Write a program to find for a given E , the longest sequence of numbers that ends with E and begins with the smallest B .
</p>
<p>
Again consider an example; if E =1011122315 then the required sequence of numbers is 303355 103325 1011122315.
</p>
<h3>Input</h3>
<p>The input may contain multiple test cases.</p>
<p>Each test case contains only one input, viz., E .</p>
<p>The input terminates when a line containing 0 appears as a test case.</p>
<h3>Output</h3>
<p>
For each test case, print the longest sequence of numbers that ends with E and begins with the smallest B . Use space to separate two consecutive numbers in the sequence.
</p>

<h3>Example</h3>
<pre><b>Sample Input</b>
1011122315
22
112213
0

<b>Sample Output</b>
303355 103325 1011122315
22
13 1113 3113 2123 112213
</pre>