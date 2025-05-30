<p>In the Ancient Clash of Mystic Pandas (ACM Pandas) game, the player plays the role of a Panda Knight who needs to defend Panda Land by defeating evil Panda Wizards. As the wizards have special magical powers, they need to be defeated using specific types of Mystic Sticks (regular bamboo sticks are ineffective against them). To obtain a Mystic Stick, Panda Knight needs to craft it by infusing his regular bamboo stick with several different kinds of magic shards according to the known recipe for that particular type of Mystic Stick.</p>
<p>Normally, all kinds of shards can be purchased for 1 gold/piece from the Panda Magic Store (therefore Panda Knight will have no problem of acquiring the shards, as long as he has enough gold to buy them all from the Store). However due to the recent invasion, to conceal the shards from the incoming Panda Wizards, Panda Magic Store has packaged all the shards into inconspicuous Mystery Boxes. A Mystery Box contains a random piece of magic shard which type can��t be determined prior to buying and opening the box, which Panda Knight can also buy for the same price (1 gold/box).</p>
<p>As his Panda Knight character is not rich, Mr. Wah is concerned about the possibility that he��s unable to buy all the necessary shards due to not getting the required amount of a specific type of shard. He needs your help! Your task as Mr. Wah��s best programmer friend is to compute the probability that he will be able to get all the shards and craft the Mystic Stick, so that he can plan his playing strategy accordingly. You can safely assume that all the required shards are available on the store via the Mystery Boxes, that the boxes will only contain the needed types of shard, and that each type of shard has equal probability of being contained inside any particular Mystery Box.</p>
<h3>Input</h3>
<p>The first line of input contains an integer T (1 �� T �� 100), the number of test cases follow. Each test case begins with two integers G and N (1 �� N �� G �� 32) in one line, denoting the amount of Panda Knight��s gold and the number of needed magic shard types respectively. The next line contains N integers, denoting how many magic shards of each type (1 �� M1 �� MN �� 32, M1 + �� + MN �� G) are needed to craft the Mystic Stick.</p>
<h3>Output</h3>
<p>For each of the test cases, print the test case number followed by the probability (in percentage, correct to 6 decimal places �C Mr. Wah is paranoid about this game) that Panda Knight will be able to craft the Mystic Stick, with the format as shown by the sample output.</p>
<pre><strong>Sample Input</strong>
5 
3 2 
1 1 
8 3 
3 2 2 
10 3 
1 2 3 
7 7 
1 1 1 1 1 1 1 
32 8 
1 1 1 1 1 1 1 1 	

<strong>Output for Sample Input</strong>
Case #1: 75.000000 
Case #2: 23.472032 
Case #3: 58.934106 
Case #4: 0.611990 
Case #5: 89.127753 	 
</pre>
<p>Explanation for 1st sample test case: There are 23 = 8 possible combinations of shard types that Knight Panda can get by purchasing 3 Mystery Boxes with his available gold:</p>
<pre>1. Type 1, Type 1, Type 1 <br>2. Type 1, Type 1, Type 2 <br>3. Type 1, Type 2, Type 1 <br>4. Type 1, Type 2, Type 2 <br>5. Type 2, Type 1, Type 1 <br>6. Type 2, Type 1, Type 2 <br>7. Type 2, Type 2, Type 1 <br>8. Type 2, Type 2, Type 2 <br></pre>
<p>Since there are 6 out of 8 combinations that gives required amount of shards (at least one Type 1 shard and one Type 2 shard), the probability that Panda Knight will be able to craft the Mystic Stick is 6/8 = 75%.</p>