<p>Leonard is very fond of buying rare and expensive science fiction toys. He keeps his collection in a sequential order of the date on which the toy was bought in a special closet so that his roomie Sheldon never gets hold of his toys. But because of his bad luck Leonard once loses a bet to Sheldon and Sheldon demands a share Leonard��s toys. Since Leonard doesn��t want to loose much money, he decides upon a strategy to reduce his loss to minimum.</p>
<p>Leonard, beginning from the first toy in his closet will pick some toys, say "x" toys in sequence. Sheldon will then pick the next "x" toys (Note that Sheldon picks equal no. of toys as picked by Leonard in his move unless the remaining toys are less than "x". In that case he picks all of the remaining). This will keep going on till no more toys are left in the closet for Leonard to pick. You are given the sequence of toys with their price. Help Leonard in maximizing the total price of all toys he picks.</p>
<p>Leonard in his each turn can either pick only 1 or 2 or 3 toys ("x" described above can take value either 1, 2 or 3).</p>
<h3>Input</h3>
<p>First line specifies T, the number of test cases.</p>
<p>Each test case contains N in the first line. Second line contains N integers as described above.</p>
<h3>Output</h3>
<p>Output 1 line for each test case giving the maximum possible value of the total sum of all toys Leonard picks.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10</p>
<p>1&lt;=N&lt;=100000</p>
<p>1&lt;=Price of toys&lt;=1000000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4
5 4 3 2
6
10 8 7 11 15 20

<strong>Output:</strong>
12
53</pre>
<p><br><strong><br>Explanation:</strong></p>
<p>In 1st case, Leonard picks 3 toys in his first move with value 5,4,3 and Sheldon has no choice but to pick the last.<br>In 2nd case, Leonard picks 10, 8. Then Sheldon picks 7,11. And then Leonard picks the rest.</p>