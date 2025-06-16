<p>You just achieved the High Score on your favorite video game! Now, you get to enter your name! You have to use the controller to enter your name, which can be awkward. Here¡¯s how it works:</p>
<ul>
<li>There are only the 26 capital letters A to Z, in order. There are no numbers, spaces, lower case letters, or any other characters.</li>
<li>Pushing UP or DOWN changes the active letter one letter forward (UP) or backward (DOWN). The active letter starts at A. It will not reset when you move around in the name. It also wraps: UP from Z goes to A, DOWN from A goes to Z.</li>
<li>Pushing LEFT or RIGHT moves the cursor one letter left or right in the current name. Note that once the cursor is at either end of the current name, it cannot move any further in that direction.</li>
<li>Pushing the FIRE button adds the active letter to the name.</li>
</ul>
<p>For example, consider the name ¡®ALMA¡¯. One way you could enter ¡®ALMA¡¯ is like this:</p>
<p style="text-align: center;"><img src="../../content/joshkirstein:55" alt="" width="598" height="246"></p>
<p style="text-align: left;">This would take 28 button pushes. However, consider entering ¡®ALMA¡¯ like this:</p>
<p style="text-align: center;"><img src="../../content/joshkirstein:56" alt="" width="595" height="247"></p>
<p style="text-align: left;">This takes only 17 button pushes. Given a name, what is the fewest number of button pushes needed to enter that name? Assume that the active letter starts at A, and that it doesn¡¯t matter where the cursor ends up when you¡¯re done.</p>
<h3>Input</h3>
<p>There will be several test cases in the input. Each test case will consist of a single string on its own line, with from 1 to 18 capital letters, representing a name that must be entered into the High Score list. The input will end with a line with a single 0.</p>
<h3>Output</h3>
<p>For each test case, output a single integer representing the smallest number of button pushes needed to enter the name. Output no spaces, and do not separate answers with blank lines.</p>
<h3>Example Input</h3>
<pre>ALMA <br>YES <br>0</pre>
<h3>Example Output</h3>
<pre>17<br>21&nbsp;</pre>