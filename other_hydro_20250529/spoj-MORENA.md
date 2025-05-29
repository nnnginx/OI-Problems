<p>&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Brunette's Candy Shop ( Easy )</span></span></strong></p>
<p style="margin-bottom: 0in; text-align: left;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">HARDER VERSION: <a href="../HILO/">http://www.spoj.com/problems/HILO/</a></span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Brunette's is a big candy shop from Little Campina in Paraibas/Brazil. This company is known for making the best candies in the world. Matheus Pheverso is the president of this company and he has a sister called Morena who loves and helps him in running the company. She uses to go the supermarket every day and buy a lot of stuffs to make all the candies. But she's insane and likes to take an alternate path to go to the supermarket.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Given the streets heights, a path is alternate only if the differences between succesive numbers strictly alternate between positive and negative.</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Ex:</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">- Street Heights: {1,3,4,5,2,9,8,10}</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">- Alternate Paths: {1,3,2,9,8}, {1,4,2,8} {1,5,2,9,8} </span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Matheus Pheverso is a friendly brother and he would like to know the longest alternate path between the first supermarket and the last supermarket, this means that his sister always starts at the supermarket number 1, and always ends at the last supermarket.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Given the number of supermarkets, and their heights, your task is to print the longest alternate path between the first and the last city.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Input</span></span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> There is a single positive integer N on the first line of input ( 1 &lt;= N &lt;= 10^6 ) representing the number of supermarkets. In the second line there're N integers Ai representing the heights of each supermarket ( -10^18 &lt;= Ai &lt;= 10^18 ).</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Ouput</span></span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> You have to print the longest alternate path between the first and the last supermarket. The supermarket number 1 is always the first, and the supermarket number N is always the last one.</span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Example</span></span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Input:</span></span></strong></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">5</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1 2 3 4 5</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Output</span></span></strong></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">2</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Input:</span></span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">8</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1 4 2 10 1 9 7 8</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: x-small;"><strong><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Output</span></span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">8</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> </span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p>&nbsp;</p>