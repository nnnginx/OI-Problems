<p><img src="./23015/file/XfWnmUPR.png">
</p><p>Shuffling the pixels in a bitmap image sometimes yields random looking images. However, by repeating the shuffling enough times, one finally recovers the original images. This should be no surprise, since "shuffling" means applying a one-to-one mapping (or permutation) over the cells of the image, which come in finite number. 

</p><p>Your program should read a number n , and a series of elementary transformations that define a "shuffling" <img src="./23015/file/k9n0dUuD.png"> of n * n images. Then, your program should compute the minimal number m (m &gt; 0) , such that m applications of <img src="./23015/file/OlztqZrC.png"> always yield the original n * n image.

</p><p>For instance if <img src="./23015/file/M71Pk83j.png"> is counter-clockwise 90<sup>o</sup> rotation then m = 4.

</p><p><img src="./23015/file/Q2Jui6vq.png"></p>
<h3>Input</h3>

<p>Test cases are given one after another, and a single 0 denotes the end of the input. For each test case:

</p><p>Input is made of two lines, the first line is number n (2 &lt;= n &lt;= 2<sup>10</sup> , n even). The number n is the size of images, one image is represented internally by a n * n pixel matrix (a<sup>j</sup><sub>i</sub>) , where i is the row number and j is the column number. The pixel at the upper left corner is at row 0 and column 0. 

</p><p>The second line is a non-empty list of at most 32 words, separated by spaces. Valid words are the keywords <b>id</b>, <b>rot</b>, <b>sym</b>, <b>bhsym</b>, <b>bvsym</b>, <b>div</b> and <b>mix</b>, or a keyword followed by <b>-</b>. Each keyword <b>key</b> designates an elementary transform (as defined by Figure 1), and <b>key-</b> designates the inverse of transform <b>key</b>. For instance, <b>rot-</b> is the inverse of counter-clockwise 90<sup>o</sup> rotation, that is clockwise 90<sup>o</sup> rotation. Finally, the list k<sub>1</sub>, k<sub>2</sub>, ..., k<sub>p</sub> designates the compound transform <img src="./23015/file/I9HiEB4F.png"> = k<sub>1</sub>ok<sub>2</sub>o ... ok<sub>p</sub> . For instance, "bvsym rot-" is the transform that first performs clockwise 90o rotation and then vertical symmetry on the lower half of the image. 

</p><p><img src="./23015/file/s9x7r4ZL.png">

</p><p>Figure 1: Transformations of image (a<sup>j</sup><sub>i</sub>) into image (b<sup>j</sup><sub>i</sub>)

</p><p><img src="./23015/file/aZubklk1.png"></p>

<h3>Output</h3>
<p>For each test case:
</p><p>Your program should output a single line whose contents is the minimal number m (m &gt; 0) such that <img src="./23015/file/EwyDJbhR.png"> is the identity. You may assume that, for all test input, you have m &lt; 2<sup>31</sup>.</p>

<h3>Example</h3>
<pre><b>Input:</b>
256
rot- div rot div
256
bvsym div mix
0

<b>Output:</b>
8
63457
</pre>