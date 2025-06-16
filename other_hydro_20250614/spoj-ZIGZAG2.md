<p>We say that a sequence of numbers x(1),x(2),...,x(k) is zigzag if no three of its consecutive elements create a nonincreasing or nondecreasing sequence. More precisely, for all i=1,2,...,k-2 either x(i+1)&lt;x(i),x(i+2) or x(i+1)&gt;x(i),x(i+2).</p>
<p>You are given two sequences of numbers a(1),a(2),...,a(n) and b(1),b(2),...,b(m). The problem is to compute the length of their longest common zigzag subsequence.  In other words, you're going to delete elements from the two  sequences so that they are equal, and so that they're a zigzag sequence. If the minimum number of elements required to do this is k then your answer is m+n-2k.</p>
<h3>Input</h3>
<p>There is a single integer t (t��100) on the first line of input. Then t test cases follow. Each of them consists of two lines. The first line contains the length of the first sequence n (1��n��2000) and n integers a(1),a(2),...,a(n). The second line contains the length of the second sequence m (1��m��2000) and m integers b(1),b(2),...,b(m). All a(i) and b(i) are from [-10<sup>9</sup>,10<sup>9</sup>].  (REPEAT: the first number on the line is not part of the sequence,  it's the length of the sequence.)</p>
<h3>Output</h3>
<p>For each test case output one line containing the length of the longest common zigzag subsequence of a and b.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 1 2 5 4 3
5 4 1 2 5 3
3 1 2 1
2 1 1
<strong>Output:</strong>
3
2
</pre>