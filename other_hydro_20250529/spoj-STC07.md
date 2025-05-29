<p>A railroad siding consists of two (dead-end) sidetracks 1 and 2. The siding is entered by track A, and left by track B.</p>

<img src="./24470/file/1lsFP5SL.png">

<p>There are N&nbsp;cars on track A, numbered from 1&nbsp;to N. They are arranged in such a way that they enter the siding in the order a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ..., a<span><sub>N</sub></span>. The cars are to be transferred to the siding, so that they leave it by track B in the order 1, 2, 3, ..., N. Each car is to be transferred once from track A to one of the sidetracks 1 or 2, and later (possibly after some transfers of the remaining cars) once from that sidetrack to the track B. The sidetracks are long enough to store even the longest trains, so there is no need to worry about their capacity.</p>
<h2>Input</h2>
<p>The first line of the standard input holds one integer N&nbsp;(1 &lt;= N &lt;= 10<sup>5</sup>) that denotes the number of cars for transfer. The second line stores the numbers a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ..., a<sub>N</sub>&nbsp;that are a permutation of 1, 2, 3, ..., N&nbsp;(i.e., each a<sub>i</sub>&nbsp;belongs to {1, 2, 3, ..., N}, and all these numbers are unique), separated by single spaces.</p>
<h2>Output</h2>
<p>The first line of the standard output should contain the word&nbsp;<tt>TAK</tt>&nbsp;(<em>yes</em>&nbsp;in Polish) if there is a way of transferring the cars so that they enter track B in the order 1, 2, 3, ..., N, or the word&nbsp;<tt>NIE</tt>&nbsp;(<em>no</em>&nbsp;in Polish) if it is impossible. If the answer is&nbsp;<tt>TAK</tt>, the second line should give, separated by single spaces, the numbers of sidetracks (1 or 2) to which successive cars a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ..., a<sub>N</sub>&nbsp;are moved in a correct transfer. If there are several ways of making the transfer, choose lexicographically smallest.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>4
1 3 4 2</pre>
<p>the correct result is:</p>
<pre>TAK
1 1 2 1</pre>
<p>And for the input:</p>
<pre>4
2 3 4 1</pre>
<p>the correct result is:</p>
<pre>NIE</pre>
<p><strong><br></strong></p>