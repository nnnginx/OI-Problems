<p>LoadingTime got a RNG (<em>Random Number Generator</em>) from his classmate several weeks ago. And he spent a lot of time study it. He found that RNG can generate a real number in range [-<b>S</b>,<b>S</b>] by executing following steps. First RNG generates n integer <b>X</b><sub>1</sub>..<b>X</b><sub>n</sub>, the sum of which is equal to <b>S</b>. Then for each <b>X</b><sub>i</sub>, it generates a real number in range [-<b>X</b><sub>i</sub>,<b>X</b><sub>i</sub>] randomly. The output (a real number) of RNG will be the sum of the <b>N</b> generated real numbers. LoadingTime noticed that the distribution of the output was very interesting, and he wanted to know: for given <b>N</b> and <b>X</b>, what's the probability that the generated number is in range [<b>A</b>,<b>B</b>]. Could you help him? 
</p><h3>Input</h3>
<p>The first line contains an integer T representing the number of test cases.
</p><p>For each test case, the first line contains three integers <b>N</b>, <b>A</b>, <b>B</b>(1 �� <b>N</b> �� 10, -100 �� <b>A</b> �� <b>B</b> �� 100) In the second line of the test case, you are given  <b>X</b><sub>1</sub>...<b>X</b><sub>n</sub>(1 �� <b>X</b><sub>i</sub> �� 10).
</p><h3>Output</h3>
<p>For each test case, print a line contains a real number representing the probablity as the problem required. It must be printed with exactly nine decimal places.
</p><h3>Example</h3>

<pre><b>Input:</b>
5
1 -100 100
10
1 10 90
10
1 -20 5
10
2 -20 5
5 5
5 -5 10
1 2 3 4 5

<b>Output:</b>
1.000000000
0.000000000
0.750000000
0.875000000
0.864720052

</pre>