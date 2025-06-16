<p>Duck is a busy guy who has <strong>N</strong> tasks to do in a single day, each task has four sub tasks. The i-th task is scheduled at the <strong>S<sub>i</sub></strong> second starting from 00:00:00, for example, 65 is 00:01:05 and 82800 is 23:00:00, and its j-th sub task requires <strong>D<sub>i,j</sub></strong> seconds to complete. That is, the j-th sub task of i-th task ends at S<sub>i</sub> + D<sub>i,j</sub> second. Duck plans to buy some machines to help him complete the tasks automatically. One machine can only deal with one task at the same time, but can deal with all four sub tasks simultaneously. Therefore, if any of the sub tasks of that task is not finished, the machine cannot deal with next task. If the whole task is finished, it can deal with the next task immediately without waiting.</p>
<p>However, Duck doesn't want that happens because he wants the machines to be more durable. He wants to maximize the cooling time of each machine whenever it completes a task. Given that the maximum cooling time of each machine is 86400, no matters at what second a machine completes a task, but the cooling time must be the same for all machines. What is the maximum cooling time that every machine can have if Duck uses as few machines as possible to complete all tasks by distributing it optimally?</p>
<h3>Input</h3>
<p>The first line is the number of test cases <strong>T</strong>. (1&nbsp;¡Ü T ¡Ü 20)</p>
<p>For each test case, it starts with the number of tasks <strong>N</strong>. (1 ¡Ü N ¡Ü 100)</p>
<p>Following N lines, each consisting of five integers: the second counting from 00:00:00 that the i-th task is scheduled at <strong>S</strong><sub><strong>i</strong></sub>, the seconds requried to complete the j-th sub task <strong>D<sub>1</sub></strong>, <strong>D<sub>2</sub></strong>, <strong>D<sub>3</sub></strong>, <strong>D<sub>4</sub></strong>.&nbsp;(1 ¡Ü S<sub>i</sub> ¡Ü 86399, 1 ¡Ü D<sub>i,</sub><sub>j</sub> ¡Ü 86400 - S<sub>i</sub>)</p>
<h3>Output</h3>
<p>Output the maximum cooling time that every machine can have.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
6
39999 7643 9987 13924 694
2000 3100 3804 2010 1999
4900 15238 28098 27777 27777
28813 11186 15742 886 20016
70000 200 300 400 500
51234 3555 30 7000 24567
3
52024 10000 7321 8864 20
62024 7321 10000 20 8864
72024 20 8864 10000 7321
</pre>
<pre><strong>Output:</strong>
2405
0
</pre>
<h3>Explanation</h3>
<p>In case 1, Duck needs two machines for task {2, 4, 6} and {1, 3, 5}, the answer is then 2405 choosing the cooling time of 2405 and 7322.</p>
<p>In case 2, one machine is enough but there is no gap between each task.</p>