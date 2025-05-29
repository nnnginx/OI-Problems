<p>You are travelling to Kullu Manili, a hill station in India. You saw some huge mountains and very curious to climb the highest ones. Assume that there are <strong>n</strong>&nbsp;mountains of height <strong>hi</strong>&nbsp;given.</p>
<p>But you were wondering about what could be the total height i need to climb if I climb only the mountain of maximum height only in a segment of k continuous mountains, considering all k segements possible. You want to calculate this for all k, such that 1&lt;=k&lt;=n.</p>
<p>Mathematically, we need to find the sum of maximum element in each possible continuous segment of size k.</p>
<h3>Input</h3>
<p>The first line contains an input <strong>n</strong>.</p>
<p>Then <strong>n</strong>&nbsp;numbers follow, denoting the height of <strong>ith</strong>&nbsp;mountain.</p>
<h3>Output</h3>
<p>Output <strong>n</strong>&nbsp;lines, where ith line contains the sum of height of mountains to climb considering all continuous segments of size <strong>i</strong>.</p>
<h3>Constraints:</h3>
<p>1&lt;=n&lt;=10000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5</pre>
<pre>5 3 4 2 3

<strong>Output:</strong>
17</pre>
<pre>16</pre>
<pre>13</pre>
<pre>9</pre>
<pre>5</pre>
<pre><strong>Explanation:</strong></pre>
<pre>For k=1, all the contiguous segments are (5), (3), (4), (2), (3). The total sum of maximum in each segment is 17 (5+3+4+2+3).</pre>
<pre>For k=2, all the contiguous segments are (5,3), (3,4), (4,2), (2,3). The total sum of maximum in each segment is 16 (5+4+4+3).</pre>
<pre>For k=3, all the contiguous segments are (5,3,4), (3,4,2), (4,2,3). The total sum of maximum in each segment is 13 (5+4+4).</pre>
<pre><span style="white-space: pre;">For k=4, all the contiguous segments are (5,3,4,2), (3,4,2,3). The total sum of maximum in each segment is 9 (5+4).</span></pre>
<pre><span style="white-space: pre;"><span style="white-space: pre;">For k=5, all the contiguous segments are (5,3,4,2,3). The total sum of maximum in each segment is 5 (5).</span></span></pre>