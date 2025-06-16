<p>&nbsp;</p>
<div style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; background-image: initial; background-attachment: initial; background-origin: initial; background-clip: initial; background-color: #ffffff; margin: 8px;">
<div style="background-image: initial; background-attachment: initial; background-origin: initial; background-clip: initial; background-color: #ffffff; margin: 8px;">
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;"><span style="font-size: small; text-align: justify;">You are going to construct a new factory in your city. Since you have major electric needs,&nbsp;</span><span style="font-size: small; text-align: justify;">having the factory placed close to a power plant is important. You want to build a prioritized&nbsp;</span><span style="font-size: small; text-align: justify;">list of possible locations.</span></p>
<p style="text-align: justify;"><span style="font-size: small;">The area in which the factory needs to be located can be represented as a rectangular grid of&nbsp;<span>N rows and M columns of cells. Some of those cells contain a power plant. The new factory&nbsp;</span><span>occupies exactly one cell, and can be placed in any empty cell (i.e., any cell that does not&nbsp;</span><span>contain a power plant).</span></span></p>
<p style="text-align: justify;"><span style="font-size: small;">Numbering rows from 1 to N and columns from 1 to M, the location of a cell can be described&nbsp;<span>by two integers. Cell (i, j) is the cell in row i and column j. The distance between cell (i0, j0)&nbsp;</span><span>and cell (i1, j1) is max(|i0 − i1|, |j0 − j1|) where |x| represents the absolute value of x. The&nbsp;</span><span>electric priority of a location is its minimum distance to a power plant.</span></span></p>
<p style="text-align: justify;"><span style="font-size: small;">With this in mind, you will number all possible locations with consecutive integers starting from &nbsp;<span>1. You will do it in ascending order of electric priority. Among locations with the same electric&nbsp;</span><span>priority, you will number them in ascending order of their row numbers. Among locations with&nbsp;</span><span>the same electric priority and row number, you will list them in ascending order of column&nbsp;</span><span>numbers.</span></span></p>
<p style="text-align: justify;"><span style="font-size: small;">In the following picture you can see a 4 × 7 grid. Black cells are the cells in which there is a&nbsp;<span>power plant. Dark gray cells have an electric priority of 1, light gray cells an electric priority of&nbsp;</span><span>2 and white cells an electric priority of 3. The number inside each cell is the number assigned&nbsp;</span><span>by you to the location.</span></span></p>
<p style="text-align: center;"><span style="font-size: small;"><span><img src="../../../content/rlewon:MELAR10" alt="" width="319" height="156"></span></span></p>
<p style="text-align: justify;"><span style="font-size: small;">&nbsp;</span></p>
<p style="text-align: justify;"><span><span style="font-size: small;">You will receive several queries about the prioritized list built. In each query you will be given&nbsp;</span></span><span><span style="font-size: small;">a number representing a position in the prioritized list and you have to calculate which location&nbsp;</span></span><span><span style="font-size: small;">was assigned the given position.</span></span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">Gene and Gina have a particular kind of farm. Instead of growing animals and vegetables, as</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">it is usually the case in regular farms, they grow strings. A string is a sequence of characters.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">Strings have the particularity that, as they grow, they add characters to the left and/or to the</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">right of themselves, but they never lose characters, nor insert new characters in the middle.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">Gene and Gina have a collection of photos of some strings at diﬀerent times during their growth.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">The problem is that the collection is not annotated, so they forgot to which string each photo</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">belongs to. They want to put together a wall to illustrate strings growing procedures, but they</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">need your help to ﬁnd an appropriate sequence of photos.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">Each photo illustrates a string. The sequence of photos must be such that if si comes imme-</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">diately before si+1 in the sequence, then si+1 is a string that may have grown from si (i.e., si</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">appears as a consecutive substring of si+1). Also, they do not want to use repeated pictures,</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">so all strings in the sequence must be diﬀerent.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">Given a set of strings representing all available photos, your job is to calculate the size of the</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 448px; width: 1px; height: 1px; overflow: hidden; color: #000000; border: 1px dashed #bbbbbb;"><span style="font-size: small;">largest sequence they can produce following the guidelines above.</span></div>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; text-align: justify;">&nbsp;</p>
<h1 style="font-size: 2em; text-align: center; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">Input</h1>
<p>&nbsp;</p>
<p style="text-align: justify;"><span style="font-size: small;">Each test case is given using several lines. The ﬁrst line contains three integers N, M and P,&nbsp;<span>representing the number of rows and columns of the grid (1 ≤ N,M ≤ 10^9</span><span>) and the number&nbsp;</span><span>of existing power plants (1 ≤ P ≤ 20). Each of the next P lines contains two integers R and&nbsp;</span><span>C representing the row and column numbers of the location of a power plant (1 ≤ R ≤ N and&nbsp;</span><span>1 ≤ C ≤ M). Within each test case, all power plant locations are diﬀerent. The next line&nbsp;</span><span>contains a single integer Q representing the number of queries (1 ≤ Q ≤ 50). Then follows a&nbsp;</span><span>line with Q integers p1, ..., pQ representing positions in the prioritized list (1 ≤ pi ≤ N×M−P).</span></span></p>
<p>&nbsp;</p>
<p style="text-align: justify;"><span style="font-size: small;">The last test case is followed by a line containing three zeros.</span></p>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
<h1 style="font-size: 2em; text-align: center; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">Output</h1>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;"><span><span style="font-size: small;">For each test case output Q + 1 lines. Line i of the ﬁrst Q lines must contain two integers&nbsp;</span></span><span><span style="font-size: small;">representing the row and column numbers of the location that was assigned number pi. The&nbsp;</span></span><span><span style="font-size: small;">last line for each test case must contain a single character ‘-’ (hyphen).</span></span></p>
<p>&nbsp;</p>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
<h1 style="font-size: 2em; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; text-align: center;">Sample</h1>
<pre style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px; text-align: justify; margin: 8px;"><span style="font-size: x-small;"><strong><span style="font-size: small;">input</span></strong><br></span><span style="font-size: small;">4 7 2
2 5
4 4
6
1 6 11 16 21 26
1000000000 1000000000 1
1 1
1
999999999999999999
0 0 0</span><span style="font-size: x-small;"><br><br></span><strong><span style="font-size: small;">output</span></strong><span style="font-size: x-small;"><br></span><span style="font-size: small;">1 4
3 3
4 5
2 7
4 7
4 1
-
1000000000 1000000000
-</span></pre>
<p style="color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px;">&nbsp;</p>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
<p style="font-size: 10px; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif;">&nbsp;</p>
</div>
</div>
<p>&nbsp;</p>