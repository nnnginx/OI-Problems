<h3>Problem</h3>
<p align="justify">
Your task will be to calculate number of different assignments of n different topics to n students such that everybody gets exactly one topic he likes.
</p>
<h3>Input</h3>
<p align="justify">
First line of input contains number of test cases c (1&lt;=c&lt;=80). Each test case begins with number of students n (1&lt;=n&lt;=20). Each of the next n lines contains n integers describing preferences of one student. 1 at the ith position means that this student likes ith topic, 0 means that he definitely doesn't want to take it.
</p>
<h3>Output</h3>
<p align="justify">
For each test case output number of different assignments (it will fit in a signed 64-bit integer).
</p>
<h3>Example</h3>
<pre>Input:
3
3
1 1 1
1 1 1
1 1 1
11
1 0 0 1 0 0 0 0 0 1 1 
1 1 1 1 1 0 1 0 1 0 0 
1 0 0 1 0 0 1 1 0 1 0 
1 0 1 1 1 0 1 1 0 1 1 
0 1 1 1 0 1 0 0 1 1 1 
1 1 1 0 0 1 0 0 0 0 0 
0 0 0 0 1 0 1 0 0 0 1 
1 0 1 1 0 0 0 0 0 0 1 
0 0 1 0 1 1 0 0 0 1 1 
1 1 1 0 0 0 1 0 1 0 1 
1 0 0 0 1 1 1 1 0 0 0 
11
0 1 1 1 0 1 0 0 0 1 0 
0 0 1 1 1 1 1 1 1 1 1 
1 1 0 1 0 0 0 0 0 1 0 
0 1 0 1 0 1 0 1 0 1 1 
1 0 0 1 0 0 0 0 1 0 1 
0 0 1 0 1 1 0 0 0 0 1 
1 0 1 0 1 1 1 0 1 1 0 
1 0 1 1 0 1 1 0 0 1 0 
0 0 1 1 0 1 1 1 1 1 1 
0 1 0 0 0 0 0 0 0 1 1 
0 1 1 0 0 0 0 0 1 0 1 

Output:
6
7588
7426

</pre>