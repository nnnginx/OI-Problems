<p><img title="FACE THE MATE" src="./22358/file/YBQloHRh.png" alt="Hero Heroine" width="462" height="301"><br>Hero and Heroine are standing on a 2D plane. Hero is standing at (x1,y1) facing towards (u1,v1) and the heroine is standing at (x2,y2) facing towards (u2,v2), both trying to find the location of the other one. Both of them are lazy and they don't move. Instead, they just change the direction they face, standing at the same position. To make things easier, both of them starts scanning simultaneously with same rotation speed. To make things even more easier, assume that they choose the direction which will help to find their mate as fast as possible. Print "Hero" if the Hero finds Heroine faster; print "Heroine" if the Heroine finds Hero faster. Print "0" otherwise.</p>
<p>Assume that both of them don't have any <a href="http://en.wikipedia.org/wiki/Field_of_view">field of view</a> and all they can see are the points in the straight line that they face.</p>
<p><strong>Input:</strong></p>
<p>The first line consists of an integer t, the number of test cases. For each test case, the first line consists of 8 non-negative integers x1,y1,u1,v1,x2,y2,u2 and v2.</p>
<p><strong>Output:</strong></p>
<p>For each test case, print the result in the required format as specified in the problem statement.</p>
<p><strong>Input Constraints:</strong></p>
<p>1&lt;=t&lt;=500000</p>
<p>0&lt;=xi,yi,ui,vi&lt;=100</p>
<p>(x1,y1) != (x2,y2) Both players are located at different positions.</p>
<p>(x1,y1) != (u1,v1)</p>
<p>(x2,y2) != (u2,v2) Players don't face their own locations.</p>
<p><strong>Sample Input:</strong></p>
<p>&nbsp;</p>
<pre>10
9 3 6 0 4 4 6 6
1 8 6 3 4 9 7 8
8 2 3 5 9 1 9 8
4 0 3 6 7 6 1 5
4 2 7 3 0 9 7 2
6 0 5 7 1 6 5 4
1 2 1 4 0 0 6 0
7 1 7 7 7 7 3 3
5 9 1 8 9 8 2 6
6 0 0 1 3 8 2 5
</pre>
<p><strong>Sample Output:</strong></p>
<p>&nbsp;</p>
<pre>0
Hero
Heroine
Hero
Heroine
Heroine
Heroine
Hero
Heroine
Heroine
</pre>