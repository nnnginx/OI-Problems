<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MTRAIN/en/">English</a></td> 
<td width="50%"><a href="/problems/MTRAIN/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Mirko and Slavko have finally gotten jobs as locomotive drivers on 
the Croatian Railroad. As early as the first day of work, they got an 
assignment. Each of them was to take their locomotive from a certain
town and visit as many towns as possible. </p><p>
Mirko is an experienced driver, so he is afraid of nothing. 
This was, however, Slavko¡¯s first train ride and he can do absolutely 
nothing by himself. Luckily, all the locomotives have radios, so Slavko 
can drive the locomotive normally as long as he is within the range 
of Mirko¡¯s radio to give him instructions. </p><p>
N towns have been given in a coordinate plane. Some of the towns are 
connected by railroad. Mirko and Slavku start their tour in different 
towns, and so that they are at most D kilometers away from each other. </p><p>
The locomotives can use all railroads, at any speed and in any 
direction. Locomotives can switch railroad tracks in towns only. 
Mirko and Slavko may be at most D kilometers away from each other at
any moment in time. </p><p>
Write a program that will determine all possible towns that Slavko 
can visit, as was described above. 
</p><p>
</p><h3>Input</h3>
<p></p><p>
The first line of the input file contains the numbers N and P, and 
a real number D, 2 ¡Ü N ¡Ü 100, 1 ¡Ü P ¡Ü 3000, 1 ¡Ü D ¡Ü 10,000. 
The number N is the number of towns, the number P is the number of 
railroads, and D is the range of the radio in kilometers (a decimal 
number two digits precise). The towns are numbered 1 to N. Each of 
the following N lines contains data describing one town, i.e. two 
integers, X and Y, -5000 ¡Ü X, Y ¡Ü 5000, representing the town¡¯s coordinates. </p><p>
Each of the following P lines contains data describing one railroad 
track, i.e. two integers G1 and G2, saying there is a railroad 
track connecting G1 i G2. </p><p>
The next line contains the starting positions of Mirko and Slavku, 
the integers U and V. Mirko starts from town U, Slavko from town V. 
U and V will represent two towns separated at most D kilometers 
in distance.
</p><p>
</p><h3>Output</h3>
<p></p><p>
The output file should contain the numbers of all the towns Slavko 
can reach. These numbers should be sorted in increasing order, each of 
them written on a separate line. </p><p>
</p><h3>Sample</h3>
<pre>vokitoki.in 
 
5 4 1.5 
0 1 
0 0 
4 1 
4 0 
2 2 
1 3 
1 5 
3 5 
2 4 
2 1 
 
vokitoki.out 
 
1 
3

vokitoki.in 
 
8 6 4 
0 0 
4 3 
8 0 
16 0 
0 -1 
8 -1 
12 -4 
16 -1 
1 2 
2 3 
3 4 
5 6 
6 7 
7 8 
1 5 
 
vokitoki.out 
 
5 
6 
7 
8 

vokitoki.in 
 
8 6 2 
0 0 
1 0 
2 0 
1 1 
0 1 
1 3 
2 1 
1 -10 
1 2 
2 4 
2 3 
5 6 
6 7 
2 8 
5 1 
 
vokitoki.out 
 
1 
2 
3 
4  
</pre>