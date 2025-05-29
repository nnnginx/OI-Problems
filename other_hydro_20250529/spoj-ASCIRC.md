<p align="justify">Bytetel Company decided to improve computers they produce. They want to replace assembler programs with special systems called assembler circuits. Assembler programs consist solely of assignments. Each assignment is determined by four elements:</p>
<div align="justify">
<ul>
        <li align="justify">two registers from which data are taken, </li>
        <li align="justify">elementary operation that should be performed on the data, </li>
        <li align="justify">register to which the result should be written. </li>
</ul>
</div>
<p align="justify">We assume that there are at most 26 registers. They are represented by small letters of English alphabet. There are at most 4 elementary operations and they are represented by capital letters A, B, C, D.</p>
<p align="justify">An assembler circuit has: </p>
<div align="justify">
<ul>
        <li align="justify">inputs assigned to registers; initial value of appropriate register is passed to the input; </li>
        <li align="justify">outputs, also assigned to registers; their final values are passed to these registers. </li>
</ul>
</div><p align="justify">There are gates inside a circuit. Each gate has two inputs and one output. The gate performs an elementary operation on data delivered on its inputs and passes the result to its output. Inputs of gates and outputs of the whole circuit are connected to outputs of other gates or inputs of the circuit. Outputs of gates and inputs of the circuit can be connected to many inputs of other gates or outputs of the circuit. Connections among gates cannot form cycles. </p>
<p align="justify">An assembler circuit is equivalent to an assembler program if for any initial state of registers the final state of registers produced by the program and the circuit are the same. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads a description of an assembler program; </li>
        <li align="justify">computes the minimal number of gates in an assembler circuit equivalent to the given program; </li>
        <li align="justify">writes the result.</li>
</ul></div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of each test case there is one integer <i>n</i> (1 &lt;= <i>n</i> &lt;= 1000), which is the number of instructions in the program. </p>
<p align="justify">In the following <i>n</i> lines there are descriptions of consecutive instructions in the program. Each description is a four-letter word beginning with an elementary operation symbol: A, B, C or D. The second and the third letter (which are small letters of English alphabet) are names of registers, in which data are placed. The fourth letter is a name of a register, in which the result should be placed. </p>

<h3>Output</h3>
<p align="justify">For each test case you should output one line with the minimal number of gates in an assembler circuit equivalent to the given program. </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
8
Afbc
Bfbd
Cddd
Bcbc
Afcc
Afbf
Cfbb
Dfdb

<b><tt>Sample output:</tt></b>
6
</pre>
<p align="justify">A circuit equivalent to the given program is shown in the figure. </p>
<p align="center"><img src="/content/ahven:uklasm.gif"></p>