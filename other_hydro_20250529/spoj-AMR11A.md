<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: x-small;">Thanks a lot for helping Harry Potter in finding the Sorcerer's Stone of Immortality in October. Did we not tell you that it was just an online game ? uhhh! now here is the real onsite task for Harry. You are given a magrid S ( a magic grid ) having R rows and C columns. Each cell in this magrid has either a Hungarian horntail dragon that our intrepid hero has to defeat, or a flask of magic potion that his teacher Snape has left for him. A dragon at a cell (i,j) takes away |S[i][j]| strength points from him, and a potion at a cell (i,j) increases Harry's strength by S[i][j]. If his strength drops to 0 or less at any point during his journey, Harry dies, and no magical stone can revive him.</span></div>
<p><span style="font-size: x-small;"> </span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 8px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Harry starts from the top-left corner cell (1,1) and the Sorcerer's Stone is in the bottom-right corner cell (R,C). From a cell (i,j), Harry can only move either one cell down or right i.e., to cell (i+1,j) or cell (i,j+1) and he can not move outside the magrid. Harry has used magic before starting his journey to determine which cell contains what, but lacks the basic simple mathematical skill to determine what minimum strength he needs to start with to collect the Sorcerer's Stone. Please help him once again.</div>
<p>Thanks a lot for helping Harry Potter in finding the Sorcerer's Stone of Immortality in October. Did we not tell you that it was just an online game ? uhhh! now here is the real onsite task for Harry. You are given a magrid S ( a magic grid ) having R rows and C columns. Each cell in this magrid has either a Hungarian horntail dragon that our intrepid hero has to defeat, or a flask of magic potion that his teacher Snape has left for him. A dragon at a cell (i,j) takes away |S[i][j]| strength points from him, and a potion at a cell (i,j) increases Harry's strength by S[i][j]. If his strength drops to 0 or less at any point during his journey, Harry dies, and no magical stone can revive him.</p>
<p>Harry starts from the top-left corner cell (1,1) and the Sorcerer's Stone is in the bottom-right corner cell (R,C). From a cell (i,j), Harry can only move either one cell down or right i.e., to cell (i+1,j) or cell (i,j+1) and he can not move outside the magrid. Harry has used magic before starting his journey to determine which cell contains what, but lacks the basic simple mathematical skill to determine what minimum strength he needs to start with to collect the Sorcerer's Stone. Please help him once again.</p>
<p>&nbsp;</p>
<h2 style="text-align: left;">Input (STDIN):</h2>
<p style="font-family: 'Times New Roman'; font-size: medium;" align="justify">The first line contains the number of test cases T. T cases follow. Each test case consists of R C in the first line followed by the description of the grid in R lines, each containing C integers. Rows are numbered 1 to R from top to bottom and columns are numbered 1 to C from left to right. Cells with S[i][j] &lt; 0 contain dragons, others contain magic potions.</p>
<h2 style="text-align: left;">Output (STDOUT):</h2>
<p style="font-family: 'Times New Roman'; font-size: medium;" align="justify">Output T lines, one for each case containing the minimum strength Harry should start with from the cell (1,1) to have a positive strength through out his journey to the cell (R,C).</p>
<h2 style="text-align: left;">Constraints:</h2>
<p>1 �� T �� 5</p>
<p>2 �� R, C �� 500</p>
<p>-10^3 �� S[i][j] �� 10^3</p>
<p>S[1][1] = S[R][C] = 0</p>
<p>&nbsp;</p>
<h2 style="text-align: left;">Sample Input:</h2>
<p><span style="font-size: medium; font-family: 'Courier New', Courier, monospace;">3<br>2 3<br>0 1 -3<br>1 -2 0<br>2 2<br>0 1<br>2 0<br>3 4<br>0 -2 -3 1<br>-1 4 0 -2<br>1 -2 -3 0</span></p>
<p>&nbsp;</p>
<h2 style="text-align: left;">Sample Output:</h2>
<p><span style="font-size: medium; font-family: 'Courier New', Courier, monospace;">2<br>1<br>2<br></span><br style="font-family: 'Times New Roman'; font-size: medium;"></p>
<h2 style="text-align: left;">Explanation:</h2>
<p>Case 1 : If Harry starts with strength = 1 at cell (1,1), he cannot maintain a positive strength in any possible path. He needs at least strength = 2 initially.</p>
<p>Case 2 : Note that to start from (1,1) he needs at least strength = 1.</p>