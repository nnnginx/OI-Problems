<p>

Mansur plays the new computer strategic game. The main task in such games is mining resources.
<br>
Fortunately in this game only one resource is necessary for development ¡ª the gold, and also there is one supplementary resource type ¡ª energy.
<br>
In this game there are mining camps, which provide certain amount of gold and energy. §¡ll camps are located along the straight line.
<br>
To protect the mining camps one can build a forcefield (a closed line contiguos segment containing mining camps) , which needs energy amount equal to it¡¯s length. 
<br>
( if  forcefield  start camp is located at X1 and  its end camp is at X2 energy needed for the whole forcefield is |X1-X2| )
<br>
Mansur wants to build one forcefield in such way, that energy of protected mining camps is enough for the forcefield, and amount of gold provided by these mining camps is maximal possible.
<br>
Write a program to help Mansur find the maximal amount of gold which he can obtain from protected mining camps.
<br>


</p><h3>Input</h3>
<p>
First line of the input file contains one integer N ¡ª number of mining camps. 
<br>
N&lt;=10^5
<br>
Following N lines contain:
<br>
three space separated integers xi, gi, di, 0 &lt;= xi &lt;= 10^9, 1 &lt;= gi &lt;= 10^9, 1 &lt;= di &lt;= 10^9: mine coordinates,amount of gold and energy provided by the mine. All xi are different and given in increasing order.
<br>


</p><h3>Output</h3>
Output only one number ¡ª maximal amount of gold which Mansur can mine.
<br>

<pre><b>Input:</b>
4 <br>
0 5 1 <br>
1 7 2 <br>
4 4 1 <br>
7 15 1 <br>

<b>Output:</b>
16
<br>
<br>
The Forcefield is camps [1,3] energy is 1+2+1=4 &gt;= 4-0 so answer is 5+4+7=16
<br>
</pre>