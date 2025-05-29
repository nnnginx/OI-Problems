<p><a href="../../../users/danish037/">Danish</a> has just solved the problem <a href="../RMID/">Running Median</a>.</p>
<p>The first line of the problem says "You will be given some integers in non-decreasing order". The problem asks you to report and remove the median of the list every time it is queried.</p>
<p>Having solved this problem, Danish now begins to wonder how to solve the problem if the input is in any order (not necessarily non-decreasing order as mentioned above).</p>
<p>Can you help him?</p>
<p>Your task is to take as input a list of positive integers. Whenever -1 is given as input, you must output the median of the list, and remove it from the list. Take the smaller element as the median in case of even number of elements.</p>
<h3>Input</h3>
<p>The input contains several test caes.</p>
<p>The first line contains an integer t, the number of test cases.</p>
<p>Each test case has several lines, each containing an integer n (&lt;=10^9) . If n is positive, add it to the list. n=-1 indicates a median query (there will be no median query if the list is empty). The test case is terminated by n=0.</p>
<p>In each test case, there will be upto 10^5 integers to be added to the list, and upto 10^5 median queries.</p>
<h3>Output</h3>
<p>For each median query as described above, print the median on a new line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
9
10
2
5
1
18
-1
-1
4
3
-1
8
7
-1
0

<strong>Output:</strong>
5
9
3
7</pre>