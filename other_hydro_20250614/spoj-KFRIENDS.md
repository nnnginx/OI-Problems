<table style="width: 834px; height: 105px;" border="0">
<tbody>
<tr>
<td>
<p><img title="horse" src="./23046/file/5xR9CCNs.png" alt="horse" width="104" height="158"></p>
</td>
<td>
<p>Gurram land is the city of Knights and is shaped exactly like a chess  board. Some of the cells in this city contains Knights. Due to scarcity  of grass ( Global Warming ! ), there has been fights between  every pair of neighboring Knights. Knight A is a neighbor of Knight B, if A can reach B in exactly one step ( see  notes for clarity ) .</p>
<p>To spread peace in the Gurram land, the United  Nations has organized a 'Friendship Mela' and wants to distribute  friendship neck straps to the Knights. Each pair of neighboring Knights then exchange Neck Strap of same color and wear it around their neck, to promote friendship :). To make it more colorful, the UN  also wants each Knight to have distinct colored neck straps around  its neck. The UN is ready to produce any number of straps of a particular color,  but can you help them to find out the minimum number of colors to be  used.</p>
<p><strong>Notes:</strong> A Knight in cell (x,y) can move in one step to any of the  cells   (x+2,y+1) , (x+2,y-1) , (x+1,y+2) , (x+1,y-2) , (x-2,y+1) ,  (x-2,y-1) ,   (x-1,y+2) , (x-1,y-2) i.e., the normal rule in standard  chess.</p>
</td>
</tr>
</tbody>
</table>
<h3>Input</h3>
<p>First line contains T ( around 10 ), the number of test cases. Each test case starts with an integer N ( 0 &lt;= N &lt;= 10000 ) the number of Knights in the city. Each of the next N lines contains two integers X Y the row and the column number of a Knight ( 1 &lt;= X,Y &lt;= 100 ). No two Knights are on a same cell.</p>
<h3>Output</h3>
<p>For each test case, print the minimum number of colors needed, in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>3<br>1 1<br>2 3<br>3 2<br>4<br>1 1<br>2 3<br>2 1<br>1 3<br><strong>Output:</strong><br>2<br>1<br><br>Case 1 : (1,1) &amp; (2,3) can exchange a Red strap , (1,1) &amp; (3,2) can exchange a Green Strap<br>Case 2 : (1,1) &amp; (2,3) can exchange a Red strap , (2,1) &amp; (1,3) can exchange a Red Strap</pre>