<p>Cradi and Vank are very fond of tiles.They have rectagular tiles of breadth 1 cm (black or white)and 2 cm (only black),with  any possible length greater than zero in infinite supply.<br> They try to make different arrangements using the tiles available to them. Two arrangements are considered same if (with or without rotation) all the tiles sizes and colors overlap with no mismatch.<br> They initially have a square tile of dimension (1 cm X 1 cm) of grey color which they call 0-layer arrangement. <br> They can add new layers of tiles keeping in mind the following constraints: <br> After completing any i layer arrangement : <br>1) Use 2 black and 2 white tiles of breadth 1 cm with length 2i + 1 and 2i + 3 to get an (i + 1)-layer arrangement. <br>2) Use 4 black tiles of breadth 2 cm with length 2i + 1 or 2i + 5 to get an (i + 2)-layer arrangement.<br> All this is done keeping in mind that adjacent tiles of same layer cannot have same color, unless they are all of 2 cm breadth (then they are all black). Some possible 2 layer arrangements are shown in the figure.</p>
<p style="text-align: center;"><img src="./24670/file/ssjn5bay.png" alt="" width="600" height="240"></p>
<p>In their desire to explore different arrangements they stumble across this strange question as to how many different n-layer aggangements are possible for any given n. Your job is to find the answer to this query.  Since the answer can be very large , print the answer modulo (10^9 + 7).</p>
<h3>Input</h3>
<p>First line contains T i.e the number of test cases. Then T line follow each containing n.</p>
<h3>Output</h3>
<p>Print the answer for each n.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
0
1
2
<strong>Output:</strong>
1
2
9
</pre>
<h4>Constraints</h4>
<p>t &lt;= 1000 <br> 0 &lt;= n &lt;= 1000000</p>