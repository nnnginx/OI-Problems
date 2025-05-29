<p style="text-align: justify;"><em>Along the skirts of the Dead Marshes I followed it, and then I had him. Lurking by a stagnant mere, peering in the water as the dark eve fell, I caught him, Gollum. He was covered with green slime. He will never love me, I fear; for he bit me, and I was not gentle. Nothing more did I ever get from his mouth than the marks of his teeth.</em></p>
<p style="text-align: right;"><em><br>¡°The Lord of the Rings: The fellowship of the Ring¡±</em></p>
<p>&nbsp;</p>
<p>Hearing Gandalf¡¯s advice, Aragorn has started hunting creature Gollum. After several days following his footprints, he has arrived to the Dead Marshes. He has a map of the marshes, that can be viewed as an M<sub>1</sub> * M<sub>2</sub> matrix containing lowercase letters form English alphabet (i.e. letters from ¡®a¡¯ to ¡®z¡¯).</p>
<p>Being a skilled ranger, Aragorn has been able to fully characterize Gollum preferred place (if you are interested, you should know that it must be dark, wet, creepy and full of fishes!). It can be described as an N<sub>1</sub> * N<sub>2</sub> matrix containing lowercase letters form English alphabet.</p>
<p>Your task is simple: write a program that, given Gollum¡¯s preferred place description and Aragorn¡¯s map, output all possible locations of the creature.</p>
<p>Let¡¯s look at an example: suppose Gollum¡¯s preferred place is described by the following 3 * 3 matrix:</p>
<p>aba</p>
<p>bab</p>
<p>aba</p>
<p>and that Aragorn¡¯s map looks something like this:</p>
<p>aababa</p>
<p>ababab</p>
<p>bababa</p>
<p>ababab</p>
<p>ababab</p>
<p>bababa</p>
<p>ababab</p>
<p>Then your program must output the following: (1,2), (1,4), (2,1), (2,3), (5,1) and (5,3), these being the upper-left corners of all places on the Dead Marshes that match Gollum¡¯s preferred place description. If none match is found, you should output the string ¡°NO MATCH FOUND...¡± without the quotes.</p>
<h3>Input</h3>
<p>Line 1: Two integers: N<sub>1</sub> and N<sub>2</sub>.</p>
<p>Lines 2¡­ N<sub>1</sub> + 1: A string with N<sub>2</sub> characters as described above.</p>
<p>Lines N<sub>1</sub> + 2: Two integers: M<sub>1</sub> and M<sub>2</sub>.</p>
<p>Lines N<sub>1</sub> + 3¡­ N<sub>1</sub> + M<sub>1</sub> + 3: A string with M<sub>2</sub> characters as described above.</p>
<p><strong>Restrictions</strong></p>
<p><br>1 ¡Ü N<sub>1</sub>, N<sub>2</sub> ¡Ü 300</p>
<p>1 ¡Ü M<sub>1</sub> * M<sub>2</sub> ¡Ü 2000</p>
<p>N<sub>1</sub> ¡Ü M<sub>1</sub></p>
<p>N<sub>2</sub> ¡Ü M<sub>2</sub></p>
<h3>Output</h3>
<p>On each line print the upper-left corner of all places that match Gollum¡¯s preferred place description on the form ¡°(x,y)¡± without the quotes, where x stands for the row and y for the column. They should be lexicographically sorted, i.e. imagine them as an ordered pair. Then (x<sub>1</sub>,y<sub>1</sub>) &lt; (x<sub>2</sub>,y<sub>2</sub>) if and only if x<sub>1</sub> &lt; x<sub>2</sub> or, if they are equal, y<sub>1</sub> &lt; y<sub>2</sub>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><p>3 3</p><p>aba</p><p>bab</p><p>aba</p><p>7 6</p><p>aababa</p><p>ababab</p><p>bababa</p><p>ababab</p><p>ababab</p><p>bababa</p><p>ababab</p><br><strong>Output:</strong><br><p>(1,2)</p><p>(1,4)</p><p>(2,1)</p><p>(2,3)</p><p>(5,1)</p><p>(5,3)</p></pre>