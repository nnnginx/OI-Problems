<p>Martin has just been hired as a computer administrator in a big  company. The company did not change its authorization system since 1980s. Every person has a four-digit personal identification number (PIN).  Nobody uses usernames or passwords, you can login just by typing your PIN. As the company grew, they added the possibility to use letters as well,  but the length of the PIN remained the same.</p>
<p>Martin is not happy with the situation. Suppose there are people  whose PINs differ only at a single place, for example <tt>61ab</tt> and <tt>62ab</tt>.  If the first person accidentally  presses 2 instead of 1, the system would still let him in. Martin would  like to make the statistics about the PINs currently in use, in particular,  compute the number of pairs of PINs that differ at 1, 2, 3 or 4 positions. He hopes that these numbers will be alarming enough to  convince his boss to invest in a better system.</p>
<p><a id="Task_specification" name="Task_specification"></a></p>
<h2><strong><span>Task specification</span></strong></h2>
<p>Given the list of PINs and an integer <span><em>D</em></span>,  find the number of pairs of PINs that  differ at exactly <span><em>D</em></span> positions.</p>
<p><a id="Input_specification" name="Input_specification"></a></p>
<h2><strong><span>Input specification</span></strong></h2>
<p>The first line of the input contains two space-separated positive  integers <span><em>N</em></span> and <span><em>D</em></span>, where <span><em>N</em></span> is the number of PINs and <span><em>D</em></span> is the  chosen number of differences.  Each of the following <span><em>N</em></span> lines  contains a single PIN.</p>
<p><a id="Constraints" name="Constraints"></a></p>
<h2><strong><span>Constraints</span></strong></h2>
<p>You may assume that in all test cases <img src="./22018/file/7WUvRQ6f.png" alt="2\leq  N\leq 50\,000"> and <img src="./22018/file/QCgKGYrf.png" alt="1 \le D \le 4">.</p>
<p>Each PIN is of length 4 and each character is either a digit or a  lowercase letter between '<tt>a</tt>' and '<tt>z</tt>', inclusive. You may assume  that all PINs in the input are different.</p>
<p>In test cases worth 15 points, <img src="./22018/file/DPenhaZo.png" alt="N\leq 2000">.</p>
<p>In test cases worth 60 points, <img src="./22018/file/JjREHfRN.png" alt="D\leq 2">. Out of those, in test cases worth 30 points, <span><em>D</em> = 1</span>.</p>
<p>In test cases worth 75 points, every PIN will only consist of  digits or lowercase letters between '<tt>a</tt>' and '<tt>f</tt>', inclusive. Thus it can be  viewed as a hexadecimal number.</p>
<p><a id="Output_specification" name="Output_specification"></a></p>
<h2><strong><span>Output specification</span></strong></h2>
<p>Output a single line with a single number: the number of pairs of  PINs that differ at <strong>exactly</strong> <span><em>D</em></span> positions.</p>
<p><a id="Examples" name="Examples"></a></p>
<h2><strong><span>Examples</span></strong></h2>
<p><strong>input:</strong></p>
<pre>4 1<br>0000<br>a010<br>0202<br>a0e2<br></pre>
<p><strong>output:</strong></p>
<pre>0<br></pre>
<p><em>For these PINs each pair of PINs differs at more than one  position.</em></p>
<p><strong>input:</strong></p>
<pre>4 2<br>0000<br>a010<br>0202<br>a0e2<br></pre>
<p><strong>output:</strong></p>
<pre>3<br></pre>
<p><em>There are three pairs that differ at exactly 2 positions: <span>(0000,<em>a</em>010)</span>, <span>(0000,0202)</span>,  and <span>(<em>a</em>010,<em>a</em>0<em>e</em>2)</span>.</em></p>