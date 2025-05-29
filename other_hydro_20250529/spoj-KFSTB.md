<h1>Help the Commander in Chief</h1>
<p>The Country of byteland is in a state of war with its neighboring nation bitland which is a small island. The king of byteland needs to send his soldiers across the sea to attack bitland. It is not easy for bytelandian soldiers to cross the sea between the two countries as there are soldiers of bitland who are constantly on patrol.</p>
<p>But, The commander of byteland through his secret sources has gathered some information about the camping spots in between, It is as follows.  There are <strong>C</strong> camping spots in the sea between the two countries. There are <strong>B</strong> <em>one way</em> bridges, each bridge is between two camps. Bytelandian army can use these bridges without any danger of being attacked. The commander also knows that if the army leaves a camping spot along a bridge safely it is not possible to  return back safely to the same camping spot.</p>
<p>The camping spot closest to the bytelandian shore is <strong>S</strong> and the camping spot closest to the bitlandian shore is <strong>T</strong>. The commander in chief of byteland wants to formulate a strategy for the army to safely move from the camping spot S to T. You have been assigned the task of finding the number of possible paths that a soldier could follow from camping spot S to T.</p>
<h3>Input</h3>
<p>The first line of input contains the number of test cases <strong>D</strong>. For each test case the first line contains C, B, S and T number of camping spots, number of one way bridges, camping spot close to byteland and camping spot close to bitland respectively. The next B lines contain description of bridges. Each bridge is described on a single line by two integers <strong>X</strong> and <strong>Y</strong> denoting the starting and ending point of a bridge.</p>
<h3>Output</h3>
<p>In each line print the number of possible paths <strong>modulo</strong> 1000000007</p>
<h3>Sample Input</h3>
<p>2<br> 4 4 1 4<br> 1 2<br> 1 3<br> 2 4<br> 3 4<br> 5 5 1 5<br> 1 2<br> 2 3<br> 2 4<br> 3 5<br> 4 5</p>
<h3>Sample Output</h3>
<p>2<br> 2</p>
<h3>Constraints</h3>
<p>1&lt;= D &lt;= 10<br> 1&lt;= C &lt;= 10000<br> 1&lt;= B &lt;= 10000<br> 1 &lt;= X,Y &lt;= C <br> 1 &lt;= S,T &lt;= C</p>