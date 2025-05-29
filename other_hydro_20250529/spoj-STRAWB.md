<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in;">Andreina the Hobbit was walking in a big yard when he saw a huge path of strawberries, Andreina ran, looking where to found her friend, Teresa (Everybody knows that Teresa LOVES strawberries), Teresa then looked the giant path of strawberries, having some amount of strawberries in a single meter, but she soon noticed that in the end of the path there was a HUGE pot of strawberries, full of this delicious fruit, Teresa, grabbed the first strawberry, but she was sent some amount of spaces ahead! However, she grabbed another strawberry and she was sent out of the range of the pot.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">She was a little confused, but, the Hobbit noticed that she was sent exactly Ai meters, the same exact amount of strawberries that were on the floor.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">Now, Teresa likes a lot this fruits and wants to reach the pot, however, she doesn't want to repeat the experience of magically sent out away from the pot! Teresa won't leave any fruits in a single square if she decides to grab it.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">Andreina the Hobbit called you, and you, the only programmer in Rainbowland must solve the problem... Andreina will give you the amount of meters to reach the pot and the number of strawberry meters that Teresa wants to pick as maximum (she has a little trauma as she was sent out of the pot range). Andreina then explains you:</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">��Teresa can grab all the strawberries in a single square, but, if she does so, she will be transported ��Ai�� meters ahead, being Ai the number of strawberries she grabbed. Else, Teresa will decide to skip the strawberry meter, she doesn't like this, so, give me the minimum strawberry meters Teresa should skip.��</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><strong>INPUT</strong>:</p>
<p style="margin-bottom: 0in;">The input will consists on T test cases, then, 3 lines will follow, the first line contains two numbers N and K, being N the number of meters and being K the maximum numbers of strawberries Teresa wants to pick, in the next line there will be N integers, giving the number of strawberries in each tile, the last number (Nn) will always be a 0, this represents the pot Teresa wants to go. Finally, the third line is a blank line.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><strong>OUTPUT</strong>:</p>
<p style="margin-bottom: 0in;">The output starts with ��Scenario #i:�� where ��i�� is the test case of evaluation starting by 1, in the next line, you should output ��Teresa will skip N strawberries�� where N is the minimum number of strawberries Teresa will skip, if Teresa should skip all the strawberries, you should output ��Teresa will skip all the strawberries��</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><strong>Sample Input</strong>:</p>
<p style="margin-bottom: 0in;">3</p>
<p style="margin-bottom: 0in;">7 2</p>
<p style="margin-bottom: 0in;">1 1 1 1 1 1 0</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">7 2</p>
<p style="margin-bottom: 0in;">3 2 1 3 2 1 0</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">7 1</p>
<p style="margin-bottom: 0in;">7 6 5 4 3 2 0</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><strong>Sample Output</strong>:</p>
<p style="margin-bottom: 0in;">Scenario #1:</p>
<p style="margin-bottom: 0in;">Teresa will skip 4 strawberries</p>
<p style="margin-bottom: 0in;">Scenario #2:</p>
<p style="margin-bottom: 0in;">Teresa will skip 0 strawberries</p>
<p style="margin-bottom: 0in;">Scenario #3:</p>
<p style="margin-bottom: 0in;">Teresa will skip all the strawberries</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><span style="text-decoration: underline;"><em>Explanation of the second sample test:</em></span></p>
<p style="margin-bottom: 0in;">Teresa takes the first strawberry at the 1st tile, moves 3 tiles to the right (4th tile), then she grabs the strawberry (3) and moves 3 more tiles, arriving then to the tile 7 where is the pot.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;"><strong>CONSTRAINTS</strong>:</p>
<p style="margin-bottom: 0in;">2&lt;=N&lt;=1000</p>
<p style="margin-bottom: 0in;">0&lt;=K&lt;=N</p>
<p style="margin-bottom: 0in;">1&lt;=Ni&lt;=N</p>