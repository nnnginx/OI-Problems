<p>World Soccer Championship is coming soon and coach Yogi wants to prepare his team as well as possible. So he made up a strategy field plan for every player of the team. One plan describes a number of possible locations for the player on the field. Moreover, if Yogi wants the player to be able to move from one location <em>A</em> to another location <em>B</em> then the plan specifies the ordered pair <em>(A,B)</em>. He is sure that his team will win if the players run over the field from one location to another using only moves of the plan.</p>
<p><img src="../../../content/ak15:fieldplan.png" alt="example image" width="50%" height="50%"></p>
<p>Yogi tells every player to follow his plan and to start from a location that reaches every other location on the plan (by possibly multiple moves). However, it is quite difficult for some soccer players, simple minded as they are, to find a suitable starting location. Can you help every player to figure out the set of possible start locations?</p>
<h3>Input</h3>
<p>The first line gives the number of field plans. The input contains at most eleven field plans (what else?). Every plan starts with a line of two integers <em>N</em> and <em>M</em>, with <em>1 ¡Ü N ¡Ü 100000</em> and <em>1 ¡Ü M ¡Ü 100000</em>, giving the number of locations and the number of moves. In the following <em>M</em> lines a plan specifies moves <em>(A,B)</em> by two white space separated integers <em>0 ¡Ü A,B &lt; N</em>. The plans are separated by a blank line.</p>
<h3>Output</h3>
<p>For every plan print out all possible starting locations, sorted increasingly and one per line. If there are no possible locations to start, print <strong>Confused</strong>. Print a blank line after each plan output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 4
0 1
1 2
2 0
2 3

4 4
0 3
1 0
2 0
2 3

<strong>Output:</strong>
0
1
2

Confused

</pre>