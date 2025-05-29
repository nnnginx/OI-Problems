<p>
	We want to find out how much related are the members of a family of monsters. 
	Each monster has the same number of genes but the genes themselves may differ 
	from monster to monster. It would be nice to know how many genes any two given 
	monsters have in common. This is impossible, however, since the number of genes 
	is very large. Still, we do know the family tree (well, not actually a tree, 
	but you cannot really blame them, these are monsters, right?) and we do know 
	how the genes are inherited so we can estimate the number of common genes quite 
	well.
</p>
<p>
	The inheritance rule is very simple: if a monster C is a child of monsters A 
	and B then each gene of C is identical to the corresponding gene of either A or 
	B, each with probability 50%. Every gene of every monster is inherited 
	independently.
</p>
<p>
	Let us define the degree of relationship of monsters X and Y as the expected 
	number of common genes. For example consider a family consisting of two 
	completely unrelated (i.e. having no common genes) monsters A and B and their 
	two children C and D. How much are C and D related? Well, each of C's genes 
	comes either from A or from B, both with probability 50%. The same is true for 
	D. Thus, the probability of a given gene of C being the same as the 
	corresponding gene of D is 50%. Therefore the degree of relationship of C and D 
	(the expected number of common genes) is equal to 50% of all the genes. Note 
	that the answer would be different if A and B were related. For if A and B had 
	common genes, these would be necessarily inherited by both C and D.
</p>
<p>
Your task is to write a program that, given a family graph and a list of pairs 
of monsters, computes the degree of relationship for each of these pairs.
</p><p>
	</p><h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a family and a list of pairs of its members from the 
		standard input,
		</li><li>
		computes the degree of relationship (in percentages) for each pair on the list,
		</li><li>
			writes the result to the standard output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of the input contains two integers n and k 
	separated by a single space. Integer n (2 &lt;= n &lt;= 300) is the number of 
	members in a family. Family members are numbered arbitrarily from 1 to n. 
	Integer k (0 &lt;= k &lt;= n - 2) is the number of monsters that do have 
	parents (all the other monsters were created by gods and are completely 
	unrelated to each other).
</p>
<p>
	Each of the next k lines contains three different integers a, b, c separated by 
	single spaces. The triple a, b, c means that the monster a is a child of 
	monsters b and c.
</p>
<p>
	The next input line contains an integer m (1 &lt;= m &lt; = n<sup>2</sup>) - 
	the number of pairs of monsters on the list. Each of the next m lines contains 
	two integers separated by a single space - these are the numbers of two 
	monsters.
</p>
<p>
	You may assume that no monster is its own ancestor. You should not make any 
	additional assumptions on the input data. In particular, you should not assume 
	that there exists any valid sex assignment.
</p>
<h3>Output</h3>
<p>
	For each test case the output consists of m lines. The i-th line corresponds to 
	the i-th pair on the list and should contain single number followed by the 
	percentage sign. The number should be the exact degree of relationship (in 
	percentages) of the monsters in the i-th pair. Unsignificant zeroes are not 
	allowed in the output (please note however that there must be at least one 
	digit before the period sign so for example the leading zero in number 0.1 is 
	significant and you cannot print it as .1). Confront the example output for the 
	details of the output format.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
7 4
4 1 2
5 2 3
6 4 5
7 5 6
4
1 2
2 6
7 5
3 3

<b><tt>Sample output:</tt></b>
0%
50%
81.25%
100%
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>