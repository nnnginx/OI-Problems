<p>In a small Village near the Himalayas, there is a rich Land-Owner, in Possession of a vast, rectangular tract of land. Unknown to him, a Major Oil Corporation has verified the existence of a vast Oil Resource beneath the land owned by him.<br><br>

The Oil Company sends a Man to negotiate the purchase of a rectangular field from within the landowner's land, with sides parallel to those of his area. The Landowner, valuing his land according to the trees growing in it and the area to be purchased, gives the company man a Map of his Land, marking the location of trees of different types, and a list of the worth of each type of tree.<br><br>

To ensure the most economic purchase of land with the required dimensions, the Company Man provides you with the
data in his possession, and alongwith that, a list of the land areas that he considers good by his judgement. <br><br>

You must provide, for each land area that he has listed, the Sum Total of the values of the Trees that lie Within or On the Boundary of that land area.<br><br>


</p><h3>Input</h3>
<p>The first line of the input contains an integer T, which is the number of test cases. For each test case, the first line contains an integer n, equal to the number of trees in the area. This line is followed by n lines each containing 3 integers separated by spaces which are coordinate of the tree ( x, y ) and value of that tree. Following this is an integer R, equal to the number of proposols of land areas given by the Company Man. Next R lines contain 4 integers each (x1, y1, x2, y2) which are the coordinates of lower left ( x1,y1 ) and upper right ( x2, y2 ) corner of the rectangular area.

</p><h3>Output</h3>
<p>For each test case, your program should output R lines containing the sum of values of the Trees which lie inside or on the corresponding rectangular plot. There should NOT BE any blank lines between output of different test cases.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
3
1 1 2
2 2 3
3 3 4
2
1 1 1 2
0 0 5 5

<b>Output:</b>
2
9
</pre>


<h3>Constraints and Limits</h3>
<p>T ¡Ü 10, n ¡Ü 10^5, r ¡Ü 50000, 0 ¡Ü x,y ¡Ü 10^7, value of any tree ¡Ü 10^4.<br>
For any rectangular area 0 ¡Ü x1 ¡Ü x2 ¡Ü 10^7, 0 ¡Ü y1 ¡Ü y2 ¡Ü 10^7<br>
<b>Note 1: </b> There can be more than one trees at the same point.<br>
<b> Note 2:</b> The input data is large ( about 15 MB ), Be careful about your input output routines.<br>.

</p>