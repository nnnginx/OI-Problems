<p>
	Every computer science student knows binary trees. Here is one of many possible 
	definitions of binary trees. Binary trees are defined inductively. A binary 
	tree t is either an external node (leaf) <img src="/content/adrian:WDOT.png" alt="o"> 
	or an ordered pair t = (t<sub>1</sub>, t<sub>2</sub>) representing an internal 
	node <img src="/content/adrian:BDOT.png" alt="*"> with two subtrees attached, left 
	subtree t<sub>1</sub> and right subtree t<sub>2</sub>. Under this definition 
	the number of nodes in any binary tree is odd. Given an odd integer n let B(n) 
	denote the set of all binary trees with n nodes, both internal and external. 
	For instance B(1) consists of only one tree <img src="/content/adrian:WDOT.png" alt="o">, 
	B(3) = {(<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">)} 
	and B(5) = {(<img src="/content/adrian:WDOT.png" alt="o">, (<img src="/content/adrian:WDOT.png" alt="o">,
	<img src="/content/adrian:WDOT.png" alt="o">)), ((<img src="/content/adrian:WDOT.png" alt="o">,
	<img src="/content/adrian:WDOT.png" alt="o">), <img src="/content/adrian:WDOT.png" alt="o">)}. 
	The trees of B(5) are depicted in the figure below.
</p>
<img src="/content/adrian:TREE2.png" alt="The trees B(5)">
<p>
	Denote by |t| the number of nodes in a tree t. Given a tree t we define its 
	unique integer identifier N (t) as follows:
</p>
<div align="justify">
	<ul>
		<li>
			N (<img src="/content/adrian:WDOT.png" alt="o">) = 0
		</li><li>
			N (t<sub>1</sub>, t<sub>2</sub>) = 2<sup>|t<sub>1</sub>|+|t<sub>2</sub>|</sup> + 
			2<sup>|t<sub>2</sub>|</sup> * N(t<sub>1</sub>) +N (t<sub>2</sub>)</li>
	</ul>
</div>
<p>
	For instance, N (<img src="/content/adrian:WDOT.png" alt="o">,<img src="/content/adrian:WDOT.png" alt="o">) 
	= 2<sup>2</sup> + 2<sup>1</sup> * 0 + 0 = 4, N (<img src="/content/adrian:WDOT.png" alt="o">, 
	(<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">)) 
	= 2<sup>4</sup> + 2<sup>3</sup> * 0 + 4 = 20,<br>N ((<img src="/content/adrian:WDOT.png" alt="o">,
	<img src="/content/adrian:WDOT.png" alt="o">), <img src="/content/adrian:WDOT.png" alt="o">) 
	= 2<sup>4</sup> + 2<sup>1</sup> * 4 + 0 = 24.
</p>
<p>
Consider the following linear order on all binary trees:
</p>
<p>
1) <img src="/content/adrian:WDOT.png" alt="o"> &lt; = t<br>
2) (t<sub>1</sub>, t<sub>2</sub>) &lt; = (u<sub>1</sub>, u<sub>2</sub>) when t<sub>1</sub>
&lt; u<sub>1</sub>, or t<sub>1</sub> = u<sub>1</sub> and t<sub>2</sub> &lt; = u<sub>2</sub>
</p>
<p>
In this order a single leaf <img src="/content/adrian:WDOT.png" alt="o"> is the 
smallest tree and given two nonleaf trees, the smaller one is that with the 
smaller left tree, if the left subtrees are different, and that with the 
smaller right subtree, otherwise. Hence for instance (<img src="/content/adrian:WDOT.png" alt="o">, 
(<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">)) 
&lt; ((<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">),
<img src="/content/adrian:WDOT.png" alt="o">), since we have <img src="/content/adrian:WDOT.png" alt="o">
&lt; (<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">). 
Assume now that the trees in B(n) were sorted using the relation &lt; =. Then, 
for each tree t in B(n) we define the successor of t as the tree that 
immediately follows t in B(n). If t is the largest one in B(n) then the 
successor of t is the smallest tree in set B(n). For instance, the successor of 
(<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">) 
in B(3) is the same tree (<img src="/content/adrian:WDOT.png" alt="o">, <img src="/content/adrian:WDOT.png" alt="o">) 
and the successor of (<img src="/content/adrian:WDOT.png" alt="o">, (<img src="/content/adrian:WDOT.png" alt="o">,
<img src="/content/adrian:WDOT.png" alt="o">)) in B(5) is ((<img src="/content/adrian:WDOT.png" alt="o">,
<img src="/content/adrian:WDOT.png" alt="o">), <img src="/content/adrian:WDOT.png" alt="o">). 
Given the integer identifier of some tree t can you give the identifier of the 
successor of t in B(|t|)?
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the identifier of some binary tree t,
		</li><li>
		computes the identifier of the successor of t in B(|t|),
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
	For each test case the first and only line of the input contains one integer n 
	(0 &lt;= n &lt; = 2<sup>30</sup>) - the identifier of some binary tree t.
</p>
<h3>Output</h3>
<p>
	For each test case the first and only line of the output should contain one 
	integer s - the identifier of the successor of t in B(|t|).
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
20
 
<b><tt>Sample output:</tt></b>
24
</pre>