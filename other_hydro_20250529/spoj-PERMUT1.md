<p>
	Let A = [a<sub>1</sub>,a<sub>2</sub>,...,a<sub>n</sub>] be a permutation of 
	integers 1,2,...,n. A pair of indices (i,j), 1&lt;=i&lt;=j&lt;=n, is an <i>inversion</i> 
	of the permutation A if a<sub>i</sub>&gt;a<sub>j</sub>. We are given integers n&gt;0 
	and k&gt;=0. What is the number of n-element permutations containing exactly k 
	inversions?
</p>
<p>
	For instance, the number of 4-element permutations with exactly 1 inversion 
	equals 3.
</p>
<h3>Task</h3>
<p>
	Write a program which for each data set from a sequence of several data sets:
</p>
<div align="left">
	<ul>
		<li>
		reads integers n and k from input,
		</li><li>
		computes the number of n-element permutations with exactly k inversions,
		</li><li>
		writes the result to output.
	</li></ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input file contains one integer d, 1&lt;=d&lt;=10, which is the 
	number of data sets. The data sets follow. Each data set occupies one line of 
	the input file and contains two integers n (1&lt;=n&lt;=12) and k (0&lt;=k&lt;=98) 
	separated by a single space.
</p>
<h3>Output</h3>
<p>
	The i-th line of the output file should contain one integer - the number of 
	n-element permutations with exactly k inversions.
</p>
<h3>Example</h3>
<pre><b>Sample input:</b>
1 
4 1 

<b>Sample output:</b>
3 
</pre>