<p>EMS memory (called <b>memory</b> for short) is some important resource of a computer. When a program is running, the computer must distribute the memory for it.</p>
<p>The classical memory distribution process is like the following:</p>
<div align="justify">
    <ul>
        <li>
        The basic unit of the memory is called a <b>cell</b>, each cell is assigned to a fixed integer number called its <b>address</b>. The address starts from number 0. If two cell's address numbers are two consecutive integer numbers, the two cells are called (logically) consecutive. We name the <i>s</i> consecutive cells starting from address <i>i</i> a piece whose length is <i>s</i> and first address is <i>i</i>.
        </li><li>
        Many programs need memory during their running. For each program, we need a application time <i>X</i>, a number of cells needed <i>M</i> and a running time <i>P</i> to describe it. When the program is running(during it starts running (time <i>T</i>) to <i>T+P</i>, including the left end and excluding the right end),The M cells cannot be used by other programs.
        </li><li>
        Suppose a program apply <i>M</i> cells at time <i>X</i> and its running time is <i>P</i>,then
        <div align="justify">
			<ul>
				<li>
				(A) If there is a piece in the memory at time <i>X</i>, each cell of which is not being used, and whose length is <i>M</i>, the computer will distribute these <i>M</i> cells to this program. If there are more pieces, the computer will choose the one whose first address is minimum.
				</li><li>
				(B) If such piece does not exist at time <i>X</i>, the program will be put into a queue.If after some time, there exist a piece whose length is <i>M</i> and the corresponding program is at the head of the queue, the computer will pop this program and distribute memory for it like (A) immediately. During the process of memory distribution, the programs which are not at the head of the queue cannot start to run before the one at the head of the queue.
				</li></ul>
		</div>
	</li></ul>
</div>
<h3>Input</h3>
<p>Ten test cases (given one after another, you have to process all!).For each test case:</p>
<p>The first line is a number N, which shows the number of memory cells. There addresses are 0..n-1. Less than 10000 lines follow, each contains 3 integers X, M(M&lt;=N), P describing the programs. A line containing three zeroes denotes the end of a test case. The programs have been sorted by there application time X.</p>
<p>All numbers in the input and output file will be less than 10<sup>9</sup>.</p>
<h3>Output</h3>
<p>For each test case output two lines. The first line contains a single integer, which shows the time when all the programs have been run and stops normally. The second line contains a single integer, which is the number of programs which has been put into the queue.</p>
<h3>Example</h3>
<pre><b>Input:</b>
10
1 3 10
2 4 3
3 4 4
4 1 4
5 3 4
0 0 0
[and 9 test cases more]

<b>Output:</b>
12
2
[and 9 test cases more]
</pre>