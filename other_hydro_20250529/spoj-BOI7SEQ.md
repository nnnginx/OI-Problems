<p>We are given a sequence a1 , ..., an . We can manipulate this sequence using the operation reduce(i), which replaces elements ai and ai+1 with a single element max(ai , ai+1 ), resulting in a new shorter sequence. The cost of this operation is max(ai , ai+1 ). After n−1 operations reduce, we obtain a sequence of length 1. Our task is to compute the cost of the optimal reducing scheme, i.e. the sequence of reduce operations with minimal cost leading to a sequence of length 1.</p>
<h3>Input</h3>
<p>The first line contains n (1 ≤ n ≤ 1,000,000), the length of the sequence. The following n lines contain one integer ai , the elements of the sequence (0 ≤ ai ≤ 1,000,000,000).</p>
<h3>Output</h3>
<p>In the first and only line of the output print the minimal cost of reducing the sequence to a single element.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>1<br>2<br>3<br><strong>Output:</strong>
5</pre>