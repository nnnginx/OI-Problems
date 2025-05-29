<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a> ]</strong></p>
<p>Daniela was offered a <em>Game of Thrones</em>&nbsp;coloring book. Each of the book's pages has <strong>N</strong>&nbsp;points marked on it, being these points numbered from <strong>1</strong>&nbsp;to <strong>N</strong>. The challenge is meant to be joining these points with lines in such a way that the figure of a dragon is formed. This problem would be a lot of fun if it was titled "Drawing dragons" and the main character was Daenerys Targaryen, but this is not so. The main character is not</p>
<div style="text-align: center;"><em>Daenerys Stormborn of the House Targaryen</em></div>
<div style="text-align: center;"><em>the first of her name</em></div>
<div style="text-align: center;"><em>Queen of the Andals, the Rhoynar and the First Men</em></div>
<div style="text-align: center;"><em>Lady of the Seven Kingdoms and Protector of the Realm</em></div>
<div style="text-align: center;"><em>Khaleesi of the Great Grass Sea</em></div>
<div style="text-align: center;"><em>the Unburnt</em></div>
<div style="text-align: center;"><em>Breaker of Chains</em></div>
<div style="text-align: center;"><em>Mother of Dragons</em></div>
<div style="text-align: center;"><em>Queen of Meereen</em></div>
<div style="text-align: center;"><em><br></em></div>
<div>but it's Daniela, who likes to draw triangles and study their properties. This is definitely a lot more fun than drawing dragons!</div>
<div>&nbsp;</div>
<div>Daniela is interested in similar triangles. A triangle is the figure that is formed by joining with line segments three unaligned points. Two triangles are said to be similar if the ratio between their corresponding sides' lengths are always the same. In the figure, triangles <strong>ABC</strong>&nbsp;and <strong>DEF</strong>&nbsp;are similar because <strong>AB/DE = BC/EF = CA/FD</strong>.</div>
<div>&nbsp;</div>
<div style="text-align: center;"><img title="TAP2016D" src="../../content/fidels:TAP2016D.png" alt="TAP2016D"></div>
<div>&nbsp;</div>
<div>Daniela has been looking at one of the books' pages for a while, thinking about the triangle formed by the first three points marked on it. She is wondering how many triangles similar to the one formed by these points can be formed using any three of the <strong>N</strong>&nbsp;points marked on the page. There are many points so it's going to take a while to find out the answer. She is now very sleepy, but she knows she won't be able to go to bed without knowing it. Can you help her by counting how many triangles similar to the one formed by the first three points (counting this triangle itself) can be formed by joining three points marked on the book's page? This way, she can go to bed and sleep peacefully during the long night.</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer number <strong>N</strong>, representing the number of points marked on the book's page (<strong>3 ¡Ü&nbsp;N&nbsp;¡Ü&nbsp;1000</strong>). Each of the following <strong>N</strong>&nbsp;lines contains two integer numbers, corresponding to one point marked on the page. The integer numbers in the <strong>i</strong>-th of these lines are <strong>X<sub>i</sub></strong>&nbsp;and <strong>Y<sub>i</sub></strong>, and they represent the coordinates of the <strong>i</strong>-th point in a cartesian coordinate system (<strong>-100 ¡Ü X<sub>i</sub>, Y<sub>i</sub>&nbsp;¡Ü&nbsp;100</strong>&nbsp;for <strong>i = 1, 2, ..., N</strong>). All points given in the input for a test case are distinct, and the first three points always form a triangle.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing an integer number, representing the number of triangles similar to the one formed by the first three points in the input, which can be formed by joining three of the points marked on the page (counting the triangle formed by the first three points itself).</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">6
0 0
1 1
-2 1
5 2
5 0
2 3
3
0 0
1 0
1 1
4
0 0
12 12
3 21
28 -4
4
-100 -100
-100 100
100 -100
100 100</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">2
1
3
4</span><span style="white-space: normal;">
</span></pre>