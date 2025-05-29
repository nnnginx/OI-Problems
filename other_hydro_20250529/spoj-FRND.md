<p>Q[b] has recently been visited by <strong>extraterrestrials</strong> from planet <strong>Quan_Lank</strong> , where everyone¡¯s name is a positive integer. <strong>All residents</strong> of the planet <strong>know each other</strong>. Two  Quan_Lank-ians  calculate the strength of their friendship by converting their names to binary, aligning them one under the other, and writing a digit in each column:  0 if the two binary digits in that column are equal, 1 if they differ. The binary result is then converted back to the decimal system.</p>
<p style="font-family: verdana;">For example, the friendship value of 19 and 10 equals 25:</p>
<p>1 &nbsp; 0 &nbsp; 0 &nbsp; 1 &nbsp; 1     =    19</p>
<p style="font-family: verdana;">0 &nbsp; 1 &nbsp; 0 &nbsp; 1 &nbsp; 0     =    10</p>
<p style="font-family: verdana;">-------------------</p>
<p style="font-family: verdana;">1 &nbsp; 1 &nbsp; 0 &nbsp; 0 &nbsp; 1     =    25</p>
<p>&nbsp;</p>
<p>The <strong>value of a planet</strong> in the Universe is defined as the sum of all friendship values. Q[b]  has asked you to help him compute the value of planet Quan_Lank!</p>
<p>&nbsp;</p>
<p style="font-family: verdana;"><strong>INPUT</strong></p>
<p style="font-family: verdana;">The first line of input contains the positive integer N (the number of residents of planet Quan_Lank , 1&lt;=N&lt;=10^6). <br>The next N lines contain the names of residents - positive integers smaller than 10^6, one per line.</p>
<p><strong>OUTPUT</strong></p>
<p style="font-family: verdana;">The only line of output must contain the value of planet Quan_Lank.</p>
<p style="font-family: verdana;"><strong>SAMPLE</strong></p>
<p style="font-family: verdana;"><strong>Input</strong><br> 2<br> 19<br> 10<br> <strong>Output</strong><br> 25</p>
<p style="font-family: verdana;"><strong>Input</strong></p>
<p style="font-family: verdana;">3<br> 7<br> 3<br> 5<br> <strong>Output</strong><br> 12<br><br> Second sample description: The friendship value of residents 1 and 2 equals 4, for residents 1 and 3<br> it equals 2, and for residents 2 and 3 it equals 6. The solution is 4 + 2 + 6 = 12.</p>