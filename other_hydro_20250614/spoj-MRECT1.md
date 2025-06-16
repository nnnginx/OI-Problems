<p>&nbsp;</p>
<p>   </p>
<p>&nbsp;</p>
<table style="cursor: default; width: 642px; background-color: #44c23c; border: 1px dashed #bbbbbb;" border="0">
<tbody>
<tr>
<td style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; cursor: text; text-align: center; margin: 8px; border: 1px dashed #bbbbbb;" width="50%"><a href="/problems/MRECT1/en/">English</a></td>
<td style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; cursor: text; text-align: center; margin: 8px; border: 1px dashed #bbbbbb;" width="50%"><a href="/problems/MRECT1/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p></p>
<p style="text-align: justify;">The government  is planing  to build a walkway  for  tourists  in  the middle of an oak  forest.&nbsp;The  forest can be represented as plane with N special lattice points representing oaks. &nbsp;The  walkway  is  represented  as  a  rectangle  with  sides  parallel  to  the  axes.  If  the  sides &nbsp;of  walkway rectangle intersect any oak lattice points, such oaks need to be axed down.&nbsp;</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">Oaks inside the rectangle do not represent problems and need not be cut down.&nbsp;Ljubo  is  the state secretary of Forestry and an passionate nature  lover, so he ordered  the&nbsp;secretary of Tourism to provide him with a list of P possible rectangle walkways that are attractive&nbsp;enough to draw in tourists.</p>
<p style="text-align: justify;">Ljubo plans to select the walkway that needs the smallest amount of oak trees to be cut down.&nbsp;</p>
<p style="text-align: justify;">Since we also like trees, would you be so kind and write a program that will determine the number&nbsp;of oaks that will be cut down for each walkway. Remember only  the oaks  intersecting  the sides of&nbsp;<span style="white-space: pre;">the rectangle need to be cut. </span></p>
<pre style="text-align: justify;"><h1 style="font-size: 2em; text-align: center;">Input</h1><span style="font-size: small;"><p style="text-align: justify;"><span style="font-family: 'courier new', courier;">The first line of input contains one integer N (1 ¡Ü N ¡Ü 300 000), number of oaks. </span></p><p style="text-align: justify;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">The next N lines contain two integers each X i Y (1 ¡Ü X, Y ¡Ü 10^9) coordinates of oaks. There will be at </span></span></p><p style="text-align: justify;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">most one oak on each lattice point. </span></span></span></p><p style="text-align: justify;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">The next line contains one integer P (1 ¡Ü P ¡Ü 100 000), number of walkways. </span></span></span></p><p style="text-align: justify;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">The next P lines contain four integers each X1, Y1, X2 , Y2 (1 ¡Ü X1 &lt; X2 ¡Ü 10^9, 1 ¡Ü Y1 &lt; Y2 ¡Ü 10^9) &nbsp;</span></span></span></p></span></pre>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: 'courier new', courier;">coordinates of the lower left (X1, Y1) and upper right (X2, Y2) corner of the rectangle.</span></span></span></span></p>
<p style="text-align: justify;"><span style="font-size: small;"><br></span></p>
<p style="text-align: center;"><img style="border: 0px initial initial;" src="../../../../../content/simes:MRECT1.jpg" border="0"></p>
<pre><p>&nbsp;</p><h1 style="font-size: 2em; text-align: center;">Output</h1>
<p><span style="font-size: medium;">Output P integers, one per line, the number of oaks that need to be cut down for each walkway in the 
order they are presented in the input. </span></p><h1 style="text-align: center;"><span style="font-size: large;">Sample</span></h1><span style="font-size: small;">
</span><p><span style="font-size: small;"><span style="font-family: 'courier new', courier;"> input 
 
6 
1 2 
3 2 
2 3 
2 5 
4 4 
6 3 
4 
2 2 4 4 
2 2 6 5 
3 3 5 6 
5 1 6 6 
 
output 
 
3 
4 
0 
1 </span></span></p>
<p> </p>
</pre>