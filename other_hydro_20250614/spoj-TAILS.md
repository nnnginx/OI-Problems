<p style="text-align: justify;">John and James planned to play a game with coins. John has 20 coins and he places it on the table in a random manner(i.e either with heads(1) or tails(0) facing up). John asked james to convert all heads into tails in minimum number of flips with the condition that if a coin is flipped the coins present to the right and left of the chosen coin should also be flipped.</p>
<h3>Input</h3>
<p>A single line with 20 space-separated integers</p>
<h3>Output</h3>
<p style="text-align: justify;">The minimum number of coin flips necessary to convert all heads into tails (i.e., to 0). For the inputs given, it will always be possible to find some combination of flips that will manipulate the coins to 20 tails.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>0 0 1 1 1 0 0 1 1 0 1 1 0 0 0 0 0 0 0 0<br><br><strong>Output:</strong>
3<br><br><strong>Hint </strong><br>Explanation of the sample: <br>&nbsp;<br>Flip coins 4, 9, and 11 to make them all tails: <br>0 0 1 1 1 0 0 1 1 0 1 1 0 0 0 0 0 0 0 0 [initial state] <br>0 0 0 0 0 0 0 1 1 0 1 1 0 0 0 0 0 0 0 0 [after flipping coin 4] <br>0 0 0 0 0 0 0 0 0 1 1 1 0 0 0 0 0 0 0 0 [after flipping coin 9] <br>0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 [after flipping coin 11]</pre>