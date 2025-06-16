<p style="text-align:justify">Loda and Maelk are legendary ChefCraft players. They have played so many games that this number doesn't fit in   a standard 32-bit integer type. Today Loda and Maelk are going to sort the things out and find out who is the   greatest ChefCraft player ever. So the great fight is coming. There are a lot of different heroes you may   choose to play ChefCraft. Obviously every hero has his pros and cons. Loda perfectly plays Blade Master. His   main skill is to make mirror images of himself to spoof the enemy.</p>
<p>&nbsp;</p>
<p style="text-align:justify">As every other popular game ChefCraft is played on a rectangular grid which consists of <strong>N</strong> rows and   <strong>M</strong> columns. Rows of the grid are numbered by integers from <strong>1</strong> to <strong>N</strong>. So the upper row of the   grid has number <strong>1</strong> and the lower row has number <strong>N</strong>. The same holds for columns. They are numbered   by integers from <strong>1</strong> to <strong>M</strong> such that the most left column has number <strong>1</strong> while the most right   column has number <strong>M</strong>.</p>
<p>&nbsp;</p>
<p style="text-align:justify">At the beginning of the game the only Blade Master's image stands on some starting cell <strong>(Sx, Sy)</strong> where   <strong>1 ≤ Sx ≤ N</strong> and <strong>1 ≤ Sy ≤ M</strong>. Then Loda makes <strong>T</strong> moves. Maelk knows how the   distribution of images on the grid changes after each Loda's move. This happens according to the following   rules.</p>
<p>&nbsp;</p>
<p style="text-align:justify"><strong>1.</strong> If there is an image standing on the cell <strong>(i, j)</strong> then the new images appear by the next   rules:</p>
<p>&nbsp;</p>
<ul>
<li>Let <strong>F(i, j)</strong> be the total number of images in the "cross" of the cell <strong>(i, j)</strong>. The "cross" of   the cell <strong>(i, j)</strong> is union of all cells in the <strong>i</strong>-th row of the grid and in the <strong>j</strong>-th column   of the grid. So <strong>N + M − 1</strong> cells belongs to the "cross".</li>
<li>Let <strong>X = F(i, j) mod 6</strong>, that is <strong>X</strong> is the remainder of the division of <strong>F(i, j)</strong> by   <strong>6</strong>.</li>
<li>For every possible value of <strong>X</strong> we have following values: <strong>D1</strong>, <strong>D2</strong>, <strong>P1 </strong> and   <strong>P2</strong>.</li>
<li><strong>D1</strong> and <strong>D2</strong> may be equal to one of the <strong>4</strong> values <strong>['U', 'R', 'D', 'L']</strong> and mean   some two directions. Here <strong>'U'</strong> means <strong>up</strong>, <strong>'R'</strong> means <strong>right</strong>, <strong>'D'</strong> means   <strong>down</strong> and <strong>'L'</strong> means <strong>left</strong>.</li>
<li><strong>P1</strong> and <strong>P2</strong> are integer numbers.</li>
<li>New mirror images will appear at every cell in the direction <strong>D1</strong> with the period <strong>P1</strong> starting   from cell <strong>(i, j)</strong> and in the direction <strong>D2</strong> with the period <strong>P2</strong> also starting from the cell   <strong>(i, j)</strong>. Of course, no images will appear out of the grid. For example, if <strong>D1 = 'U'</strong> and <strong>P1 =   2</strong> then images appear at the cells <strong>(i − 2, j), (i − 4, j), (i − 6, j)</strong>, and so   on.</li>
<li>Loda always use the same values for <strong>D1</strong> and <strong>D2</strong>. Namely,<br> <strong>D1 = 'U', D2 = 'D'</strong> for <strong>X = 0,</strong><br> <strong>D1 = 'L', D2 = 'R'</strong> for <strong>X = 1,</strong><br> <strong>D1 = 'U', D2 = 'R'</strong> for <strong>X = 2,</strong><br> <strong>D1 = 'R', D2 = 'D'</strong> for <strong>X = 3,</strong><br> <strong>D1 = 'D', D2 = 'L'</strong> for <strong>X = 4,</strong><br> <strong>D1 = 'L', D2 = 'U'</strong> for <strong>X = 5.</strong></li>
<li>But values <strong>P1</strong> and <strong>P2</strong> may vary for different games. But once chosen they will be the same for   all moves.</li>
</ul>
<p>&nbsp;</p>
<p style="text-align:justify"><strong>2.</strong> Appearing of new mirror images happens immediately.</p>
<p>&nbsp;</p>
<p style="text-align:justify"><strong>3.</strong> Whenever there is more than one image at the cell they start one on one fights. In each fight two   images participate and both die. So if the number of images in the cell was even than all images will   disappear in the end, otherwise exactly one image will remain at this cell.</p>
<p>&nbsp;</p>
<p style="text-align:justify">Now Maelk wants to choose his hero in order to win the fight. The most important thing he needs to know for   this is how the number of images changes during Loda's moves. So he asks you for help. Denote by <strong>C(t)</strong> the number of images on the grid after the <strong>t</strong>-th Loda's move for <strong>t</strong> from <strong>1</strong> to <strong>T</strong>. For   convenience we denote <strong>C(0) = 1</strong> with meaning that <strong>0</strong>-th move is the putting of the only Blade   Master's image at the starting cell. Maelk wants you to calculate the sum <strong>C(0) + C(1) + ... + C(T)</strong>.   Since Maelk doesn't know what to expect from Loda he would like to know the answer for several values of   <strong>T</strong>. As you remember the total number of games played by Maelk and Loda at ChefCraft doesn't fit in a   standard 32-bit integer type. Of course, the same can hold for the number of moves in their final fight. Since   Maelk plays ChefCraft the whole life he is not strong in math and can't calculate such large sums. So let's   help him to win the final fight and become the only ChefCraft master ever.</p>
<h3>Input</h3>
<p style="text-align:justify">The first line of the input contains three space separated integers <strong>N</strong>, <strong>M </strong> and <strong>Q</strong>. Here   <strong>N</strong> and <strong>M</strong> are sizes of the grid described above and <strong>Q</strong> is the number of Maelk's queries. The   second line contains two space separated integers <strong>Sx</strong> and <strong>Sy</strong>, row index and column index of the   starting position of the first image. Each of the following six lines contains two space separated integers,   the values <strong>P1</strong> and <strong>P2 </strong> for the corresponding <strong>X</strong>, that is, <strong>i</strong>-th line among these six   lines contains values <strong>P1</strong> and <strong>P2 </strong> for <strong>X = i − 1</strong>. Each of the following <strong>Q</strong> lines contains a single integer <strong>T</strong>, the number of Loda's moves for the corresponding Maelk's query.</p>
<h3>Output</h3>
<p style="text-align:justify">For every Maelk's query output on a separate line the numbers of images Maelk will see during Loda's move.</p>
<h3>Constrains</h3>
<p style="text-align:justify"><strong>N</strong> and <strong>M</strong> are positive<br> <strong>N</strong> • <strong>M</strong> ≤ <strong>34</strong><br> <strong>1</strong> ≤ <strong>Sx</strong> ≤ <strong>N</strong><br> <strong>1</strong> ≤ <strong>Sy</strong> ≤ <strong>M</strong><br> <strong>1</strong> ≤ <strong>P1</strong>, <strong>P2</strong> ≤ <strong>max{N, M}</strong><br> <strong>1</strong> ≤ <strong>Q</strong> ≤ <strong>100</strong><br> <strong>1</strong> ≤ <strong>T</strong> ≤ <strong>10<sup>16</sup></strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 3 3
1 1
1 1
1 1
1 1
1 1
1 1
1 1
1
2
3

<strong>Output:</strong>
4
12
17
</pre>
<h3>Explanation</h3>
<p style="text-align:justify">The initial grid looks as follows:<br> 100<br> 000<br> 000<br> Here '1' represents a cell with an image and '0' represents a free cell.<br> <br> After the first move grid is<br> 111<br> 000<br> 000<br> <br> After the second move grid is<br> 101<br> 111<br> 111<br> <br> Finally, after the third move we have<br> 011<br> 101<br> 010<br> <br> So after the first move Maelk will see <strong>3</strong> images, after the second move – <strong>8</strong> images and   after the third move – <strong>5</strong> images. Hence the answers for <strong>T = 1, 2, 3</strong> are <strong>1 + 3 = 4</strong>,   <strong>1 + 3 + 8 = 12</strong> and <strong>1 + 3 + 8 + 5 = 17</strong> respectively.</p>