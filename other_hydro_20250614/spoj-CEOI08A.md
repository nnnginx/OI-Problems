<p>One morning, fruit farmer Fred visits his apple trees and notices that one of them was cut overnight. This means a loss of 111e ¨C the money he can make from the apples of a tree on average. In order to prevent further losses, he decides to erect a fence on his plantation.<br>The fence consists of posts connected by wire.</p>
<p>The fence posts can only be placed at a given set of pre-drilled holes. While Fred can get wire for free, he needs to buy the fence posts for 20e each. So it might not always be worth or even possible to fence in all of his trees.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="fences" src="./21774/file/GsSBICGU.png" alt="fences" width="340" height="169"></p>
<p>The plantation is square and 1 000 ¡Á 1 000 m2 large. In bird¡¯s eye view, the lower left corner has<br>coordinates (0, 0), the upper right (1 000, 1 000). In this example there are four pre-drilled holes (circles) and three trees (squares). It is optimal to buy three fence posts and put them into selected holes (filled circles), to connect them by wire (lines), and to leave the upper left hole empty. The cost of erecting the fence is 3 ¡¤ 20e + 1 ¡¤ 111e = 171e since three posts were bought and one tree could not be fenced in (which means a loss of that tree¡¯s harvest).</p>
<p><br>Write a program that reads the positions of the pre-drilled holes and the trees on Fred¡¯s plan-tation and outputs the minimum cost of erecting a fence or erecting no fence at all. You can neglect the actual shape of the trees and calculate with their positions only.</p>
<p><strong>Input</strong></p>
<p>The first line contains two integers N and M (3 ¡Ü N ¡Ü 100, 1 ¡Ü M ¡Ü 100). N is the number of pre-drilled holes, and M is the number of trees. This line is followed by N lines that describe the positions of the holes, and then by M lines that describe the positions of the trees. Allpositions are given as pairs of integers x y on one line (0 ¡Ü x, y ¡Ü 1 000). You can expect thatno two positions (of holes and trees) coincide and that no three positions are colinear.</p>
<p><br><strong>Output</strong><br>Output a single line containing one integer: Fred¡¯s minimum cost. In case Fred buys P posts<br>and fails to fence in T trees, his cost are 20P + 111T .</p>
<p>&nbsp;</p>
<p><strong>Sample Input</strong></p>
<p>4 3<br>800 300<br>200 200<br>200 700<br>600 700<br>400 300<br>600 500<br>800 900</p>
<p><strong>Output:</strong></p>
<p>171</p>
<p>This example corresponds to the picture above.</p>
<p><strong>(Official Test Data)</strong></p>
<p>&nbsp;</p>