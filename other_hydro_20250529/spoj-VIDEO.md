<p>
Bessie is playing a video game! In the game, the three letters 'A', 'B',

and 'C' are the only valid buttons. Bessie may press the buttons in any

order she likes. However, there are only N distinct combos possible (1 &lt;= N

&lt;= 20). Combo i is represented as a string S_i which has a length between 1

and 15 and contains only the letters 'A', 'B', and 'C'.
</p>
 
<p>
Whenever Bessie presses a combination of letters that matches with a combo,

she gets one point for the combo. Combos may overlap with each other or

even finish at the same time! For example if N = 3 and the three possible

combos are "ABA", "CB", and "ABACB", and Bessie presses "ABACB", she will

end with 3 points. Bessie may score points for a single combo more than once.
</p>
 
<p>
Bessie of course wants to earn points as quickly as possible. If she

presses exactly K buttons (1 &lt;= K &lt;= 1,000), what is the maximum number of

points she can earn?
</p>


<h3>Input description</h3>

<p>
* Line 1: Two space-separated integers: N and K.<br>
* Lines 2..N+1: Line i+1 contains only the string S_i, representing combo i.<br>
</p>

<h3>Output description</h3>

<p>
* Line 1: A single integer, the maximum number of points Bessie can obtain.
</p>

<br>
<h3>Example</h3>

<pre><b><u>Input:</u></b>
3 7
ABA
CB
ABACB

<b><u>Output:</u></b>
4
</pre>


<h3>Example details</h3>
 
<p>
The optimal sequence of buttons in this case is ABACBCB, which gives 4 points:<br>
1 for ABA, 1 from ABACB, and 2 from CB.
</p>