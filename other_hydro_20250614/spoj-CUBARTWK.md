<p><em>International Center for Picassonian Cubism</em> is a Spanish national museum of cubist artworks, dedicated to Pablo Picasso. The center held a competition for an artwork that will be displayed at the facade of the museum building.</p>
<p>The artwork is a collection of cubes that are piled up on the ground and is intended to amuse visitors, who will be curious how the shape of the collectionof cubes changes when it is seen from the front and the sides. The artwork is a collection of cubes with edges of 1 foot long and is built on a ﬂat ground that is divided into a grid of unit squares, measuring 1 foot long on each side. Due to some technical reasons, cubes of the artwork must be either put on the ground, ﬁtting into a unit square in the grid, or put on another cube in the way that the bottom face of the upper cube exactly meets the top face of the lower cube. No other way of putting cubes is possible.</p>
<p>You are a member of the judging committee responsible for selecting one out of a plenty of artwork proposals ubmitted to the competition. The decision is made primarily based on artistic quality but the cost for installing the artwork is another important factor. Your task is to investigate the installation cost for each proposal. The cost is proportional to the number of cubes, so you have to ﬁgure out the minimum number of cubes needed for installation.</p>
<p>Each design proposal of an artwork consists of the front view and the side view (the view seen from the right-hand side), as shown in Figure 1.</p>
<p style="text-align: center;"><img title="Figure 1: An example of artwork proposal" src="../../../content/johnm91:figure1.png" alt="Figure 1: An example of artwork proposal" width="400" height="276"></p>
<p>The front view (resp., the side view) indicates the maximum heights of piles of cubes for each column line (resp., row line) of the grid.</p>
<p>There are several ways to install this proposal of artwork, such as follows.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="Explanation of Figure 1" src="../../../content/johnm91:figure1exp.png" alt="Explanation of Figure 1"></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;">In these ﬁgures, the dotted lines on the ground indicate the grid lines. The left ﬁgure makes use of 16 cubes, which is not optimal. That is, the artwork can be installed with a fewer number of cubes. Actually, the right one is optimal and only uses 13 cubes.</p>
<p style="text-align: left;"><br>Notice that swapping columns of cubes does not change the side view. Similary, swapping rows does not change the front view. Thus, such swaps do not change the costs of building the artworks.</p>
<p style="text-align: left;">For example, consider the artwork proposal given in Figure 2.</p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: center;"><img title="Figure 2: Another example of artwork proposal" src="../../../content/johnm91:figure2.png" alt="Figure 2: Another example of artwork proposal"></p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: left;">An optimal installation of this proposal of artwork can be achieved with 13 cubes, as shown in the following ﬁgure, which can be obtained by exchanging the rightmost two columns of the optimal installation of the artwork of Figure 1.</p>
<p style="text-align: left;">&nbsp;</p>
<p style="text-align: center;"><img title="Explanation" src="../../../content/johnm91:figure2exp.png" alt="Explanation"></p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input is a sequence of datasets. The end of the input is indicated by a line containing two<br>zeros separated by a space. Each dataset is formatted as follows.</p>
<p><br><em>w d<br>h<sub>1</sub> h<sub>2</sub> ··· h<sub>w</sub><br>h′<sub>1</sub> h′<sub>2</sub> ··· h′<sub>d</sub></em></p>
<p>The integers <em>w</em> and <em>d</em> separated by a space are the numbers of columns and rows of the grid, respectively. You may assume 1 ≤ <em>w</em> ≤ 10 and 1≤ <em>d</em> ≤ 10. The integers separated by a space in the second and third lines specify the shape of the artwork. The integers <em>h<sub>i</sub></em> (1≤ <em>hi</em> ≤ 20, 1≤<em> i </em>≤<em> w</em>) in the second line give the front view, i.e., the maximum heights of cubes per each column line, ordered from left to right (seen from the front); The integers <em>h′<sub>i</sub></em> (1≤ <em>h′<sub>i</sub></em> ≤ 20, 1≤ <em>i </em>≤ <em>d</em>) in the third line give the side view, i.e., the maximum heights of cubes per each row line, ordered from left to right (seen from the right-hand side).</p>
<h3>Output</h3>
<p>For each dataset, output a line containing the minimum number of cubes. The output should not contain any other extra characters.</p>
<p>You can assume that for each dataset there is at least one way to install the artwork.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5 5<br>1 2 3 4 5<br>1 2 3 4 5<br>5 5<br>2 5 4 1 3<br>4 1 5 3 2<br>5 5<br>1 2 3 4 5<br>3 3 3 4 5<br>3 3<br>7 7 7<br>7 7 7<br>3 3<br>4 4 4<br>4 3 4<br>4 3<br>4 2 2 4<br>4 2 1<br>4 4<br>2 8 8 8<br>2 3 8 3<br>10 10<br>9 9 9 9 9 9 9 9 9 9<br>9 9 9 9 9 9 9 9 9 9<br>10 9<br>20 1 20 20 20 20 20 18 20 20<br>20 20 20 20 7 20 20 20 20<br>0 0<br><br><strong>Output:</strong><br>15<br>15<br>21<br>21<br>15<br>13<br>32<br>90<br>186<br></pre>