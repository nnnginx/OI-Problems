<p>Once upon a time, there's a person named Tresi. He's quite old but hasn't found the love of his life. He starts to feel uncomfortable with his life. On another day, he found a magic lamp that will grant one wish for him. Of course, Tresi wishes for many girls to accompany him. Finally, Tresi has many beautiful girls that love him.</p>
<p>But since Tresi never had a girlfriend before, he's having trouble fulfilling the girls' needs. This is caused because the girls doesn't want to feel lonely or too overcrowded. Tresi has N rooms in his house. After some observation, Tresi knows that each girl will feel lonely if left in a room alone or with only one other girl. Tresi also knows that if a room contains 5 or more girls, there will be chaos in that room. Tresi doesn't want his girls to be unhappy. But, the time to move a girl to another room is one minute since Tracy have to sweet talk to the girl first. Tresi asks for your help to decide the minimum time that he must spend for the girls so they can live happily.</p>
<h3>Input</h3>
<p>First line contains a number T which is the number of test cases. Each test case consists of 2 lines. First line is N which is the number of rooms that Tresi has. Second line contains N number Bi which is the number of girls on room i.</p>
<h3>Output</h3>
<p>For each test case, output a line containing the time needed for Tresi to satisfy the girls. If Tresi can't satisfy all the girls, output "Tresi gagal memuaskan gadisnya.".</p>
<h3>Sample Input</h3>
<pre>3
3
1 2 3
5
0 3 4 3 0
3
1 1 0</pre>
<h3>Sample Output</h3>
<pre>1
0
Tresi gagal memuaskan gadisnya.</pre>
<div style="border: 1px solid #ADC; background-color: #0cc; padding: 5px; margin-bottom: 10px;">
<h3>Explanation</h3>
<ul>
<li>For the first case, Tresi can move a girl from room 1 to room 2, for a total time of 1 minute.</li>
<li>For the second case, all the girls are already happy.</li>
<li>For the third case, there aren't any configuration that can make all the girls happy.</li>
</ul>
</div>
<div style="border: 1px solid #FC0; background-color: #ffc; padding: 5px; margin-bottom: 10px;">
<h3>Constraint</h3>
<ul>
<li>1 �� T �� 10</li>
<li>1 �� N �� 100000</li>
<li>0 �� b<span style="vertical-align: sub;">i</span>&nbsp;<span style="font-size: 10.3999996185303px; background-color: #ffffcc;">��</span>&nbsp;4</li>
</ul>
</div>