<p>Tatama Land is on a crisis. Recently, a dragon woke up and will destroy Tatama Land to ashes. Hearing this news, Pheo, Waca, and Wembo decided to create a guild called Quest Hunter to slay the dragon.</p>
<p>In order to defeat the dragon, they want to buy weapons first. They visit J0I Blacksmith, which sells N weapons, each with a price of X<sub>i</sub> gold. As Quest Hunter only have Y golds, they want to buy as many weapons as they can using Y golds.</p>
<p>After buying weapons, they go to a local tavern to hire mercenaries for their guild. Each mercenary should buy a weapon they just bought. However, Quest Hunter lost the bill, and they totally forget how much gold for each weapon. They decided to randomly give a price to each weapon, but no weapon will costs 0 gold, and the total price of all weapons should be the same amount with total gold used to buy those weapons. Now, they're curious about how many price configurations available. As the answer can be very large, output it with modulo 10<sup>9</sup> + 7</p>
<h3>Input</h3>
<p>An integer T, number of test cases in the first row<br>For each testcase:<br>- First row is an integer N<br>- Second row contains N integer, X<sub>i</sub>, the price of each weapon<br>- Third row is an integer Y&nbsp;</p>
<h3>Output</h3>
<p>For each testcase, output "Case #C: D" where C is the testcase number and D is the number of configurations.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>1 2 3 4 5<br>6<br>4<br>2 2 2 2<br>1

<strong>Output:</strong>
Case #1: 3<br>Case #2: 0&nbsp;</pre>
<div style="border: 1px solid #ADC; background-color: #0cc; padding: 5px; margin-bottom: 10px;">
<h3>Explanation</h3>
<ul>
<li>For the first case, total amount of money is (1+2+3) = 6 and there are 3 weapons. Quest Hunter can sell it using these configurations (1,1,4), (1,2,3), (2,2,2)</li>
<li>For second case, Quest Hunter can't buy any weapons</li>
</ul>
</div>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>1 ¡Ü T ¡Ü 10<sup>2</sup></li>
<li>1 ¡Ü N,Y,X<sub>i</sub> ¡Ü 10<sup>3</sup></li>
</ul>
</div>