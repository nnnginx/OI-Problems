<p>There is a Chipmunk with <strong>"Brain"</strong> and he want to dig holes in a yard to store his food.<br> There is a rectangular yard which is divided into unit cells, initially having some holes<strong>(H)</strong> and sand<strong>(S)</strong>. The chipmunk can dig one row at a time, But he have to dig all the sand(S) positions simultanously and due to this holes(H) which are already there got filled with sand.<br> <br>Example:<br> Suppose a Row is <strong>"SHSHH"</strong> then after digging the row becomes <strong>"HSHSS" i.e all "S" replace with "H" and vice versa</strong>.<br> <br>Now Chipmunk wants to have a <strong>large square of holes</strong> somewhere in the yard. The sides of square must be parallel to the sides of the yard. Find a sequence of turns that produces the largest possible square of  holes somewhere in the yard and help him to find the area of that  square.</p>
<h3>Input</h3>
<p>Given two interger Rows(R) and column(C) (1&lt;=R,C&lt;=30)<br> Next line contain a RxC rectangular yard of sand (S) and hole (H).</p>
<h3>Output</h3>
<p>Print largest "Area of the Square" that can be obtain after sequence of turns.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2<br>SS<br>HH
<br><strong>Output:</strong>
4<strong><br><br>Input:</strong>
5 1<br>H<br>S<br>H<br>H<br>H
<br><strong>Output:</strong>
1</pre>