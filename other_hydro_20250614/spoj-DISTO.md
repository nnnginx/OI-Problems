<!-- p { margin-bottom: 0.08in; } -->
<p style="margin-bottom: 0in;" align="LEFT">One day, Eloy the byte was walking at the square (1,1) of the big Matrix-shaped city... He was planning to go visit his mom at the square (N,N) when some meteors crashed at the city! Every byte doesn't know what to do... Eloy rapidly discovers that the meteors cause a distortion, multiplying by his hit expansion the streets affected... Eloy knows the matrix and what is contained in it and know the places where the meteor crash, given this, determine the resultant matrix of the city.</p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT">Additional information: Every street in the initial matrix is filled with ASCII characters from '!' to '}' (from 33 to 125 in ASCII numbers).</p>
<p style="margin-bottom: 0in;" align="LEFT">The hit expansion for the meteor starts with 5, as it expands will decrease by 1 until arrives to <strong>1</strong><span style="font-weight: normal;">, this value will multiply the value of the matrix. This is a example of a hit expansion, (the meteor crashed at the position (3,3))</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><img title="Meteor Expansion" src="../../../../../../content/simes:DISTO.jpg" alt="Meteor expansion" width="708" height="146"></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> So, in the example of 'c' (position (3,3)) (99 in ASCII) you should multiply it by 5 (495). But in the magic digital world where Eloy lives, this number will be an ASCII symbol. More information on the output.</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><strong><span style="font-weight: normal;"> INPUT:</span></strong></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> First line of input contains two integers N and K</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> N Contains the size of the matrix (the matrix will be N^2) (3&lt;=N&lt;=500)</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> K Contains the number of meteors that crashed in the city. (1&lt;=K&lt;=50)</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> The next N lines contains N characters separated by a single space, this will be the content of the matrix at position (I,J)</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> The next K lines contains two integers (Ki and Kj), (Rows,Columns) this two coordinates reveal the position where meteor Kn crashed.</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><strong><span style="font-weight: normal;"> OUTPUT:</span></strong></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> The output must be the resultant matrix, so, N lines with N characters separated by a single space, as the distortion can get out of range some integers, you must output the ascii value of the number modulo 93 plus 33. That will decrease the number to a range from 33 to 125 as much. This final number must be turned into a character, then print it.</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;"> SAMPLE:</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><strong><span style="font-weight: normal;">INPUT:</span></strong></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">3 1</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">a a a</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">b b b</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">c c c</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">2 2</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><strong><span style="font-weight: normal;">OUTPUT:</span></strong></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">1 1 1</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">5 : 5</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">9 9 9</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">Because:</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">The m</span><span style="font-weight: normal;">eteor crash at (2,2) having a starting value of 98, the value in the matrix is modified to 490, then transformed to the range 33~125 giving a result of 58, in ASCII value, 58 represents the ��:��.</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">later, the hit expansion moves to EVERY ADJACENT cell (that means diagonals too) modifying the values inside of it.</span></p>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT">ANOTHER SAMPLE DATA:</p>
<p style="margin-bottom: 0in;" align="LEFT">INPUT:</p>
<p style="margin-bottom: 0in;" align="LEFT">6 1<br>a a a a a a<br>b b b b b b<br>c c c c c c<br>d d d d d d<br>e e e e e e<br>f f f f f f<br>1 6</p>
<p style="margin-bottom: 0in;" align="LEFT">OUTPUT:</p>
<p>% % ) - 1 5 <br>&amp; &amp; + 0 5 5 <br>' ' - 3 3 3 <br>( ( / / / / <br>) ) ) ) ) ) <br>* * * * * *</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-weight: normal;">Please have in consideration that if 2 meteors collide and affects the same zone (cell), the zone with the GREATEST value of modification should be modified.</span></p>