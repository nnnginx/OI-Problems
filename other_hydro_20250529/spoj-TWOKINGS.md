<p style="text-align: center;"><span style="font-size: large;"><strong><span style="font-size: medium;"><a href="http://spoj.com/problems/QWERTY04/" target="_blank"></a></span><br>TRIVIADOR</strong></span></p>
<p>Triviador is a war between two Kings. A king can attack an enemy region at each step. When a king attacks a region, he conquers all the enemy regions connected to it(not just the immediate ones). All the 8 regions around any region are connected to it. The kings get alternate chances to attack. King1 gets the chance to attack first. Assume both kings are intelligent and find who will conquer the whole territory at the end of the war. It can be proved that one of the Kings can win for sure if he is intelligent!</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Input Specification:</strong></p>
<p>The first line is an integer t, denotes the number of test cases. In each test case the first line consists of two integers denoting the number of rows and columns in the territory (each cell is a region). Then the description of each cell follows. Every region contains a character ��X�� if it is owned by king1 or ��O�� otherwise. <br> <br> <br> <strong>Output Specification</strong>:<br> For each test case output the result in a single line ��X�� if king1 wins or ��O�� if king2 wins.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Input Constraints:</strong></p>
<p><strong>T&lt;=100</strong></p>
<p><strong>1&lt;=rows,columns&lt;=10</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>Sample input:</strong></p>
<p><strong><br> </strong>3</p>
<p>3 3</p>
<p>XOX</p>
<p>XXX</p>
<p>XOX</p>
<p>&nbsp;</p>
<p>3 5</p>
<p>XXXXX</p>
<p>XXXOO</p>
<p>XXXOO</p>
<p>&nbsp;</p>
<p>4 4</p>
<p>XXXX</p>
<p>OOOO</p>
<p>XXXX</p>
<p>OOOO</p>
<p><strong><br>Sample Output:</strong></p>
<p>O</p>
<p>X</p>
<p>X</p>
<p>&nbsp;</p>
<p><strong>Explanation of testcase 1 and 2:<br></strong></p>
<p><strong>Case 1: </strong>King1 has two possibilities to attack. But after attacking any of them, he will lose surely when king2 attacks back.</p>
<p><strong>Case 2: </strong>King1 can attack any of the four enemy positions. He conquers all the connected enemy positions. So this is a one step victory.<strong> </strong></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"> </span></p>
<p><span style="font-size: small;">Try the 1D version of this problem : <a href="http://spoj.com/problems/QWERTY04/" target="_blank">http://spoj.com/problems/QWERTY04/</a><br>Try the 3D version of this problem : <a href="http://spoj.com/problems/CONQUER/">http://spoj.com/problems/CONQUER/</a></span></p>