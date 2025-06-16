<p>There are 3 kinds of animals A,B and C. A can eat B,B can eat C,C can eat A. It's 

interesting,isn't it?</p>
<p>Now we have n animals,numbered from 1 to n. Each of them is one of the 3 kinds of 

animals:A,B,C. </p>
<p>Today Mary tells us k pieces of information about these n animals. Each piece has one of 

the two forms below:
</p><div align="justify">
       <ul>
               <li>
               1 x y: It tells us the kind of x and y are the same.
               </li><li>
               2 x y: It tells us x can eat y.
               </li>
       </ul>
</div>
<p>Some of these k pieces are true,some are false. The piece is false if it satisfies one of 

the 3 conditions below, otherwise it's true.</p>
<div align="justify">
       <ul>
               <li>
               X or Y in this piece is larger than n.
               </li><li>
               This piece tells us X can eat X.
               </li><li>
               This piece conflicts to some true piece before.
               </li>
       </ul>
</div>
<h3>Input</h3>
<p>The first line contains a single integer t.t blocks follow.</p>
<p>To every block,the first line contains two integers n(1&lt;=n&lt;=50000) and k (1&lt;=k&lt;=100000).
k lines follow,each contains 3 positive integers D(1&lt;=D&lt;=2),X,Y,separated by single 

spaces.</p>
<h3>Output</h3>
<p>t lines,each contains a single integer - the number of false pieces in the corresponding block.</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
100 7
1 101 1
2 1 2
2 2 3
2 3 3
1 1 3
2 3 1
1 5 5

<b><tt>Sample output:</tt></b>
3

<b><tt>Hint:</tt></b>
<p>The false pieces are the 1st,the 4th and the 5th ones.</p>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>