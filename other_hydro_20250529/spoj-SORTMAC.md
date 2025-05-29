<p>We have a sorting machine that works on a list of distinct numbers. This machine only has two instructions, named MOVEBACK and MOVEFRONT. Each instruction takes one element of the list as a parameter and removes that element from the list. MOVEBACK will then append that element to the end of the remaining list, while MOVEFRONT will insert it at the beginning.</p>
<p>For example, the sequence {8,12,25,7,15,19} can be sorted in ascending order using 2 instructions:</p>
<ul>
<li>MOVEFRONT 7, to get {7,8,12,25,15,19}</li>
<li>MOVEBACK 25, to get {7,8,12,15,19,25}</li>
</ul>
<p>You will be given a list of distinct numbers. Compute the minimum number of instructions required to sort the list in ascending order.</p>
<h3>Input</h3>
<p>Input starts with an integer T (¡Ü 100), denoting the number of test cases.</p>
<p>Each case starts with an integer N (1 ¡Ü N ¡Ü 50), denoting the number of elements. Next line consists N distinct elements. Each element will be between -1000 and 1000.</p>
<h3>Output</h3>
<p>For each case, print one line containing the answer to the problem.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
6
8 12 25 7 15 19
5
1 2 3 4 5
5
1 -10 -1 -8 4
</pre>
<pre><strong>Output:</strong>
2
0
3
</pre>