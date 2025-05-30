<p>��There are too many numbers here!�� your boss bellows. ��How am I supposed to make sense of all of this? Pare it down! Estimate!�� You are disappointed. It took a lot of work to generate those numbers. But, you��ll do what your boss asks. You decide to estimate in the following way: You have an array A of numbers. You will partition it into k contiguous sections, which won��t necessarily be of the same size. Then, you��ll use a single number to estimate an entire section. In other words, for your array A of size n, you want to create another array B of size n, which has k contiguous sections. If i and j are in the same section, then B[i]=B[j]. You want to minimize the error, expressed as the sum of the absolute values of the differences (��|A[i]-B[i]|).</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There will be several test cases in the input. Each test case will begin with two integers on a line, n (1 �� n �� 2,000) and k (1 �� k �� 25, k �� n), where n is the size of the array, and k is the number of contiguous sections to use in estimation. The array A will be on the next n lines, one integer per line. Each integer element of A will be in the range from -10,000 to 10,000, inclusive. The input will end with a line with two 0s.</p>
<h3>Output</h3>
<p>For each test case, output a single integer on its own line, which is the minimum error you can achieve. Output no extra spaces, and do not separate answers with blank lines. All possible inputs yield answers which will fit in a signed 64-bit integer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7 2
6
5
4
3
2
1
7
0 0

<strong>Output:</strong>
9</pre>