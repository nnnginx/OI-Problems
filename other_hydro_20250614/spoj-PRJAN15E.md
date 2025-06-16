<p><span style="font-size: small;"><br></span></p>
<div>
<p><span style="font-size: small;">Mr. Kaboom has recently learned about maximum flow. Now his friend Mr. Taboom gave him this problem.</span></p>
<p><span style="font-size: small;">You are given a tree with <strong>N</strong> vertices. The vertices are numbered from <strong>1 to N</strong>.  Each edge of the tree has some capacity associated with it. Between  each pair of vertices there is only one way to go. Now imagine for each  pair of vertices that one of the vertex is the source and the other is  the sink. Then Mr. Kaboom needs to find out what is the maximum flow for  each pair of vertices. Mr. Taboom decides to reduce Mr. Kaboom's misery  and asked him to provide the sum of maximum flow between all possible  pair of vertices. Mr. Kaboom has found no solution and has trusted you  with this task. Can you save his day?</span></p>
</div>
<div><span style="font-size: small;"><br> </span>
<div>
<h3><span style="font-size: small;">Input</span></h3>
<div>
<p><span style="font-size: small;">The very first line of the input will contain the number of test cases  <strong>T</strong>. Then T tests follow. First line of each test contains <strong>N</strong>,  the number of vertices in the tree. The next N-1 lines each contain  three integers. The first two integers denotes the vertices this edge  connects. The third integer gives the capacity of the edge.</span></p>
</div>
</div>
<span style="font-size: small;"><br> </span>
<div>
<h3><span style="font-size: small;">Output</span></h3>
<div>
<p><span style="font-size: small;">For each tests output one integer per line, the sum of all pair maximum flow in the tree.</span></p>
<p><span style="font-size: small;">See the explanation of the sample for more understanding. In every pair the vertices should be different.</span></p>
<p><span style="font-size: small;">You can read about maximum flow <a href="http://en.wikipedia.org/wiki/Maximum_flow_problem">here</a> , and for tree <a href="http://en.wikipedia.org/wiki/Tree_%28data_structure%29">here</a></span></p>
</div>
</div>
<span style="font-size: small;"><br> </span>
<div>
<h3><span style="font-size: small;">Constraints</span></h3>
<div><ol>
<li><span style="font-size: small;">1��  T �� 20</span></li>
<li><span style="font-size: small;"><span style="color: #3e3f3a; line-height: 20px;">1�� N��10</span><span style="box-sizing: border-box; line-height: 0; position: relative; vertical-align: baseline; top: -0.5em; color: #3e3f3a;">5</span></span></li>
<li><span style="font-size: small;">Capacities of each edge will be non-negative and no more than 10<sup>6<sup>.</sup></sup></span></li>
<li><span style="font-size: small;">The total number of vertices among all test cases will be less than 5*10<sup>5</sup></span></li>
</ol></div>
</div>
</div>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">The total number of vertices among all test cases will be less than 500000.<br><strong>&nbsp;</strong></span></p>
<p><span style="font-size: small;"><strong>Sample Input<br></strong>2<br>4<br>1 2 5<br>1 3 2<br>1 4 3<br>3<br>1 2 5<br>2 3 6</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><strong><span style="font-size: small;">Output:</span></strong></p>
<p><span style="font-size: small;">34<br>32</span></p>
<p><strong><span style="font-size: small;">Explanation:</span></strong></p>
<div>
<p><span style="font-size: small;">For the first case, the maximum flow for each pair is,</span></p>
<p align="center"><span style="font-size: small;"><img title="source: imgur.com" src="file://O9L0Z8wM.png" alt=""></span></p>
<hr>
<p><span style="font-size: small;">For the second case, the maximum flow for each pair is,</span></p>
<p align="center"><span style="font-size: small;"><img title="source: imgur.com" src="file://F9s7seUD.png" alt=""></span></p>
<p style="text-align: left;"><strong><span style="font-size: small;">Problem-setter: Nafis Sadique</span></strong></p>
</div>