<p>In Croatia there are N small islands. For the purposes of further tourism development, the government has decided to build exactly one hotel on the each island. The government has contracts with two hotel chains: let's call them A and B. Unfortunately, there is a problem since each hotel chain wants to build as many hotels as possible.</p>
<p>Thus, the following agreement has been made: the hotels will be built such that, for each horizontal or vertical line (that is, if we imagine the problem in the 2D coordinate system, for each line with the equation y = c or x = c), the absolute difference between the number of hotels (on that line) of the chain A and the number of hotels (on that line) of the chain B is at most 1.</p>
<p>Write a program that will, for each small island, determine the hotel chain (A or B) which will build the hotel on that island, such that the upper agreement holds.</p>
<p style="text-align: center;"><span style="font-size: small;"><strong>Input</strong><strong>&nbsp;</strong></span></p>
<p>In the first line of input there is an integer T, the number of test cases.</p>
<p>For each test case, in the first line there is an integer N, the number of islands.</p>
<p>In the next line there are eight integers: X(1), Y(1), Ax, Bx, Mx, Ay, By, My; each from the interval [1, 100 000], except for X(1) and Y(1) which are from the interval [0, Mx-1] and [0, My-1], respectively.</p>
<p>2D coordinates of the i-th island (for 2 �� i �� N) are:</p>
<p>X(i) = ( Ax * X(i-1) + Bx ) mod Mx;</p>
<p>Y(i) = ( Ay * Y(i-1) + By ) mod My.</p>
<p>It is guaranteed that no two islands will have the same position and the solution, not necessarily unique, will always exist.</p>
<p><strong>Note:</strong> Author's solution doesn't depend on properties of pseudo-random generator.</p>
<p>Data set is divided into 2 parts:<br>&nbsp;&nbsp;&nbsp;&nbsp; First part: &nbsp;&nbsp;&nbsp;&nbsp;1 &lt;= T &lt;= 100, 1 &lt;= N &lt;= 5000<br>&nbsp;&nbsp;&nbsp;&nbsp; Second part: 1 &lt;= T &lt;= 10, 1 &lt;= N &lt;= 100 000</p>
<p style="text-align: center;"><span style="font-size: small;"><strong>Output</strong><strong>&nbsp;</strong></span></p>
<p>For each test case, output in a separate line a string of size N, containing only the letters A and B. The i-th letter of the string denotes the hotel chain which will build the hotel on the i-th island.</p>
<p style="text-align: center;"><span style="font-size: small;"><strong>Example</strong><strong>&nbsp;</strong></span></p>
<p><strong>Input: <br></strong></p>
<p>1<br>10<br>2 4 8 2 5 6 9 5</p>
<p><br> <strong>Output:</strong></p>
<p>AAAABBBBBA</p>
<p>&nbsp;</p>
<p><em>The points in this example are:</em></p>
<p><em>2 4<br>3 3<br>1 2<br>0 1<br>2 0<br>3 4<br>1 3<br>0 2<br>2 1<br>3 0</em></p>