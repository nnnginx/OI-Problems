<p>
	In a factory, moulds for casting metal objects are produced by a special 
	cutting device. The device is equipped with cuboid-shaped blade of size 1 mm x 
	1 mm x 30 mm (its height) which operates with each of its sides thus producing 
	the mould from cuboid of size 250 mm x 250 mm x 30 mm (its height). The end of 
	the blade newer lowers below the bottom surface of the cuboid. In any moment 
	the distance between initial and current position doesn't exceed 1000.
</p>
<p>
	The machine understands special command language which has the following 
	grammar:
	</p><pre><tt>&lt;command block&gt; ::= [ &lt;command&gt; ; {&lt;command&gt; ; } ] 
&lt;command&gt;       ::= &lt;lift&gt; | &lt;shift&gt; | &lt;command block&gt;
&lt;lift&gt;          ::= ^ &lt;distance&gt;
&lt;shift&gt;         ::= @ &lt;direction&gt; &lt;distance&gt;
&lt;direction&gt;     ::= N | S | W | E 
&lt;distance&gt;      ::= &lt;sign&gt; &lt;number&gt; | &lt;number&gt;
&lt;number&gt;        ::= &lt;digit&gt; {&lt;digit&gt;}
&lt;sign&gt;          ::= - | + 
&lt;digit&gt;         ::= 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 
</tt></pre>
<p>
	where {exp} means zero or more exps.&nbsp;
</p>
<p>
	The command &lt;lift&gt; causes moving the blade downwards when the distance is 
	a positive number and upwards otherwise. The command &lt;shift&gt; moves the 
	blade in the appropriate direction (N--north, S--south, W--west, E--east).
</p>
<h3>Task</h3>
<p>
	Write a program which for each data set from a sequence of several data sets:
</p>
<div align="justify">
	<ul>
		<li>
		reads a command block from input,
		</li><li>
		computes the volume of hollows made by the machine commanded by a given command 
		block (assuming that before the execution the blade is located 1 mm above the 
		north-west corner of the virgin cuboid),
		</li><li>
			writes the result to output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input file contains one integer d, 1 &lt;= d &lt;= 10, 
	which is the number of data sets. The data sets follow. Each data set occupies 
	one line of the input file and is a word derived from &lt;command block&gt; of 
	the above grammar of length not exceeding 10000 characters.
</p>
<h3>Output</h3>
<p>
	The i-th line of the output file should contain one integer -- the volume (in 
	cubic mm) of the hollows made by the machine controlled by the command block 
	given in the i-th data set.
</p>
<h3>Example</h3>
<pre>Sample input:

<tt>1 
[^2;@S2;] 
</tt>

Sample output:

<tt>3</tt>

</pre>