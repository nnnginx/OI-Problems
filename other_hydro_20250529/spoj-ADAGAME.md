<p>Ada the Ladybug is playing <strong>Game of Digits</strong> against her friend Velvet Mite Vinit. The game is played in following manner: At first, there is a four-digit number and a number of moves. Both Ada and Vinit take turns alternately (beginning with Ada). Both of them must increase ANY digit of the number, but if the digit was 9 it will become 0.</p>
<p>For example number 3590 can be expanded to: 4590,3690,3500 or 3591. If after all turns the number is greater than the original number, Ada wins - otherwise Vinit is the winner. Both of them play optimaly - can you decide who is the winner?</p>
<p>PS: It is possible, that Ada will have one more turn (if number of turns is odd)</p>
<h3>Input</h3>
<p>First line of input will consist <strong>T ¡Ü 200</strong> number of test-cases.  Each testcase will consist of four digit number <strong> 0 ¡Ü N &lt; 10<sup>4</sup></strong> [the original number] and <strong> 0 ¡Ü M ¡Ü 100 </strong> [the number of turns].</p>
<h3>Output</h3>
<p>For each test-case, print the name of winner ("<strong>Ada</strong>" or "<strong>Vinit</strong>").</p>
<h3>Example Input</h3>
<pre>5
0000 0
5566 3
3333 10
9999 9
1234 30
</pre>
<h3>Example Output</h3>
<pre>Vinit
Ada
Ada
Vinit
Ada
</pre>