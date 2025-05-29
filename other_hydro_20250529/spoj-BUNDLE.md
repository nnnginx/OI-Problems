<p>Outel, a famous semiconductor company, recently released a new model of 
	microprocessor called Platinium. Like many modern processors, Platinium can 
	execute many instructions in one clock step providing that there are no 
	dependencies between them (instruction I<sub>2</sub> is dependent on 
	instruction I<sub>1</sub> if for example I<sub>2</sub> reads a register that I<sub>1</sub>
	writes to). Some processors are so clever that they calculate on the fly which 
	instructions can be safely executed in parallel. Platinium however expects this 
	information to be explicitly specified. A special marker, called simply a stop, 
	inserted between two instructions indicates that some instructions after the 
	stop are possibly dependent on some instructions before the stop. In other 
	words instructions between two successive stops can be executed in parallel and 
	there should not be dependencies between them.
</p>
<p>
	Another interesting feature of Platinium is that an instruction sequence must 
	be split into groups of one, two or three successive instructions. Each group 
	has to be packed into a container called a bundle. Each bundle has 3 slots and 
	a single instruction can be put into each slot, however some slots may stay 
	empty. Each instruction is categorized into one of 10 instruction types denoted 
	by consecutive capital letters from A to J (instructions of the same type have 
	similar functionality, for example type A groups integer arithmetic 
	instructions and type F groups instructions). Only instructions of certain 
	types are allowed to be packed into one bundle. A template specifies one 
	permissible combination of instruction types within a bundle. A template can 
	also specify a position of a stop in the middle of a bundle (there is at most 
	one such stop allowed). In addition, stops are allowed between any two 
	adjoining bundles. A set of templates is called a bundling profile. When 
	packing instructions into bundles, one has to use templates from bundling 
	profile only.
</p>
<p>
	Although Platinium is equipped with an instruction cache it was found that for 
	maximal performance it is most crucial to pack instructions as densely as 
	possible. Second important thing is to use a small number of stops.
</p>
<p>
	Your task is to write a program for bundling Platinium instructions. For the 
	sake of simplicity we assume that the instructions cannot be reordered.
</p>
<h3>Task</h3>
<p>
	Write a program that:
</p>
<div align="justify">
	<ul>
		<li>
		reads a bundling profile and a sequence of instructions,
		</li><li>
		computes the minimal number of bundles into which the sequence can be packed 
		without breaking the dependencies and the minimal number of all stops that are 
		required for the minimal number of bundles,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer z, the number of test cases. Then z test 
	cases follow.
</p>
<p>
	The first line of each test case descripition contains two integers t and n 
	separated by a single space. Integer t (1 &lt;= t &lt;= 1500) is the number of 
	templates in the bundling profile. Integer n (1 &lt;= n &lt;= 100000) is the 
	number of instructions to be bundled.
</p>
<p>
	Each of the next t lines specifies one template and contains 3 capital letters 
	t<sub>1</sub>,t<sub>2</sub>,t<sub>3</sub> with no spaces in between followed by 
	a space and an integer p. Letter t<sub>i</sub> (A &lt; = t<sub>i</sub>&lt;= J) 
	is an instruction type allowed in the i-th slot. Integer p (0 &lt;= p &lt;= 2) 
	is the index of the slot after which the stop is positioned (0 means no stop 
	within the bundle).
</p>
<p>
	Each of the next n lines specifies one instruction. The i-th line of these n 
	lines contains one capital letter c<sub>i</sub> and an integer d<sub>i</sub>, 
	separated by a single space. Letter c<sub>i</sub> (A &lt;= c<sub>i</sub>&lt;=J) 
	is the type of the i-th instruction. Integer d<sub>i</sub> (0 &lt; = d<sub>i</sub>
	&lt; i) is the index of the last instruction (among the previous ones) that the 
	i-th instruction is dependent on (0 means that the instruction is not dependent 
	on any former instruction).
</p>
<p>
	You can assume that for each instruction type c describing an instruction in 
	the instruction sequence there is at least one template containing c.
</p>
<h3>Output</h3>
<p>
	For each test case, the first and only line of the output contains two integers 
	b and s. Integer b is the minimal number of bundles in a valid packing. Integer 
	s is the minimal number of all stops that are required for the minimal number 
	of bundles.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
4 9 
ABB 0 
BAD 1 
AAB 0 
ABB 2 
B 0 
B 1 
A 1 
A 1 
B 4 
D 0 
A 0 
B 3 
B 0 

<b><tt>Sample output:</tt></b> 
4 3 
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>