<p>
A computer with only one instruction!
The instruction is: 

</p><pre>SUBLEQ A B C
</pre>

<p>This means: subtract the value in M(A) from M(B) and store it in M(B); if the result is non-positive jump to the instruction in position C. M(i) represents the value stored in memory position i. The computer has a memory of 9999 integer positions, numbered from 0 to 9998. C &gt; 9996, indicates the end of the program.  Also, if A is negative, then the value of A is directly subtracted from M(B). </p><p>
Since there is only one instruction, it is unnecessary to represent its opcode explicitely in memory. Therefore, an instruction is stored in main memory using three consecutive memory positions, which correspond to the three instruction parameters.

The memory is organized as follows:

</p><pre>Position Content
0-8      input/output variables (M0 to M8)
9-9998   program memory (instructions+data)
</pre>

<p>The following pseudo-code shows the one instruction computer simulator:

</p><pre>simulate(integer M[0..9998])
   integer pc,A,B,C
   pc = 9
   while (pc&lt;9997)
      A = M[pc]; B = M[pc+1]; C = M[pc+2]
      if(A&gt;=0) 
         M[B] = M[B] - M[A]
      else
         M[B] = M[B] - A
      if (M[B]&gt;0)
         pc = pc + 3
      else
         pc = C
      end_if
   end_while
end_simulate
</pre>

<p>Each iteration of the above while instruction is called a simulation cycle.  You are to translate postfix instructions into this machine language.  There are
at most 100 arithematic terms and 99 operators. Numerical constants are non-negative and less than or equal to 10000.

</p><h3>Input</h3>
<p>The input has several test cases, one test case per line. Each test case corresponds to an arithmetic expression in postfix notation. An expression may contain constants (integer values), input variables (M0 to M8) and arithmetic operators (+, -, *, /).  

</p><h3>Output</h3>
<p>For each test case, a program must be printed using the following format: First line indicates m, the number of instructions of the program; and the following m lines contain the program, one instruction per line, where each instruction is represented by 3 integer values separated by one blank space.  Your outputed program must finish
within 10^7 simlation cycles for each test case.
</p><h3>Example</h3>

<pre><b>Input:</b>
100
M1 M2 -

<b>Output:</b>
3
0 0 12
-100 0 0
19 19 10000

4
0 0 12
1 2 15
2 0 18
21 21 10000
</pre>