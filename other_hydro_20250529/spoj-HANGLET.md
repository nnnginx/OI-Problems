<p>
	Little Tom is learning how to program. He has just written some programs but is 
	afraid to run them, because he does not know if they will ever stop. Please 
	write a program to help him. This task is not as easy as it may seem, because 
	Tom's programs are possibly not deterministic. Given a program written by Tom, 
	your program should tell him whether his program can stop and if so, what is 
	the shortest possible time before it stops.
</p>
<p>
	Tom's computer consists of 32 1-bit registers and the program consists of n 
	instructions. The registers are numbered from 0 to 31 and the instructions are 
	numbered from 0 to n-1.
</p>
<p>
	Below, MEM[a] stands for the contents of the a-th register, 0 &lt;= a, b &lt; 
	32, 0 &lt;= x &lt; n, 0 &lt;= c &lt;= 1.
</p>
<p>
	The instruction set is as follows:
</p>
<div align="left">
	<pre><tt><hr size="1">
Instruction   Semantics 
<hr size="1">
AND a b       MEM[a] := MEM[a] and MEM[b] 
OR a b        MEM[a] := MEM[a] or MEM[b] 
XOR a b       MEM[a] := MEM[a] xor MEM[b] 
NOT a         MEM[a] := not MEM[a] 
MOV a b       MEM[a] := MEM[b] 
SET a c       MEM[a] := c 
RANDOM a      MEM[a] := random value (0 or 1) 
JMP x         jump to the instruction with the number x 
JZ x a        jump to the instruction with the number x if MEM[a] = 0 
STOP          stop the program 
<hr size="1">
</tt></pre>
</div>
<p>
	The last instruction of a program is always STOP (although there can be more 
	than one STOP instruction). Every program starts with the instruction number 0. 
	Before the start, the contents of the registers can be arbitrary values. Each 
	instruction (including STOP) takes 1 processor cycle to execute.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the program,
		</li><li>
		computes the shortest possible running time of the program,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of the input contains an integer n (1 &lt;= n 
	&lt;= 16) being the number of instructions of the program. Each of the next n 
	lines contains one instruction of the program in the format given above. You 
	may assume that the only white characters in the program are single spaces 
	between successive tokens of each instruction.
</p>
<h3>Output</h3>
<p>
	For each test case the first and only line of the output should contain the 
	shortest possible running time of the program, measured in processor cycles. If 
	the program cannot stop, output should contain the word HANGS.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2
5 
SET 0 1 
JZ 4 0 
RANDOM 0 
JMP 1 
STOP 
5 
MOV 3 5 
NOT 3 
AND 3 5 
JZ 0 3 
STOP 
<b><tt>Sample output:</tt></b>
6 
HANGS
</pre>