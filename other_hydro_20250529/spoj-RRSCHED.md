<p>A computer processor is given N tasks to perform (1 ¡Ü N ¡Ü 50,000). The i-th task requires T<sub>i</sub> seconds of processing time (1 ¡Ü T<sub>i</sub> ¡Ü 1,000,000,000). The processor runs the tasks as follows: each task is run in order, from 1 to N, for 1 second, and then the processor repeats this again starting from task 1. Once a task has been completed, it will not be run in later iterations. Determine, for each task, the total running time elapsed once the task has been completed.</p>

<h3>Input</h3>
<p>The first line of the input contains the integer N, and the next N lines contain the integers T<sub>1</sub> through T<sub>N</sub>.</p>

<h3>Output</h3>
<p>Output N lines, the i-th of which contains an integer representing the time elapsed when task i has been processed.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
8
1
3
3
8

<b>Output:</b>
22
2
11
12
23
</pre>

<p>The second task is completed during the first iteration, finishing 2 seconds in. On the third iteration, the third and fourth tasks complete at 11 seconds and 12 seconds, respectively. Finally, on the eighth iteration, the first and last tasks complete at 22 seconds and 23 seconds, respectively.</p>

<center><b>Warning: large input/output data.</b></center>
<br>

<i><font size="1">Note: This problem statement is the exclusive and proprietary property of TopCoder, Inc. Any unauthorized use or reproduction of this information without the prior written consent of TopCoder, Inc. is strictly prohibited. (c)2006, TopCoder, Inc. All rights reserved.</font></i>

<p><font size="1">(See <a href="http://forums.topcoder.com/?module=Thread&amp;threadID=608536&amp;start=0&amp;mc=30#956263">this post</a> for more information.)</font></p>