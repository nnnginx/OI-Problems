<p>The ancient Babylonians decided to build a huge tower. The tower  consists of <span><em>N</em></span> cubic building blocks that are  stacked one onto another. The Babylonians gathered many building blocks  of various sizes from all over the country. From their last unsuccessful attempt they have learned that if they put a  large block directly onto a much smaller block, the tower will fall.</p>
<p><a id="Task_specification" name="Task_specification"></a></p>
<h2><strong><span>Task specification</span></strong></h2>
<p>Each two building blocks are different, even if they have the same  size. For each building block you are given its side length. You are also given an integer <span><em>D</em></span> with  the following meaning: you are not allowed to put block A directly onto block B if the side length  of A is strictly larger than <span><em>D</em></span> plus  the side length of B.</p>
<p>Compute the number of different ways in which it is possible to  build the tower using <strong>all</strong> the building blocks. Since this number can be very large, output the result modulo <span>10<sup>9</sup> + 9</span>.</p>
<p><a id="Input_specification" name="Input_specification"></a></p>
<h2><strong><span>Input specification</span></strong></h2>
<p>The first line of the input contains two positive integers <span><em>N</em></span> and <span><em>D</em></span>:   the number of building blocks and the tolerance respectively.</p>
<p>The second line contains <span><em>N</em></span> space-separated integers; each represents the size of one building block.</p>
<p><a id="Constraints" name="Constraints"></a></p>
<h2><strong><span>Constraints</span></strong></h2>
<p>All numbers in the input files are positive integers not exceeding <span>10<sup>9</sup></span>.</p>
<p><span><em>N</em></span> is always at least 2.</p>
<p>In test cases worth 70 points <span><em>N</em></span> will be at most 70.</p>
<p>Out of those, in test cases worth 45 points, <span><em>N</em></span> will be at most 20.</p>
<p>Out of those, in test cases worth 10 points, <span><em>N</em></span> will be at most 10.</p>
<p>For some of the test cases the total number of valid towers will  not exceed <img src="./22019/file/txebwdsB.png" alt="1\,000\,000">.  These test cases are worth 30 points in total.</p>
<p>For the last six test cases (worth 30 points) the value of <span><em>N</em></span> is larger than 70. No upper bound on <span><em>N</em></span> is given for these test cases.</p>
<p><a id="Output_specification" name="Output_specification"></a></p>
<h2><strong><span>Output specification</span></strong></h2>
<p>Output a single line containing a single integer: the number of  towers that can be built, modulo <img src="./22019/file/iLJL8N4G.png" alt="1\,000\,000\,009">.</p>
<p><a id="Examples" name="Examples"></a></p>
<h2><strong><span>Examples</span></strong></h2>
<p><strong><strong>input:</strong></strong></p>
<pre>4 1<br>1 2 3 100<br></pre>
<p><strong><strong>output:</strong></strong></p>
<pre>4<br></pre>
<p><em>We can arrange the first three blocks in any order, except for <span>2,1,3</span> or <span>1,3,2</span>. The  last block has to be at the bottom.</em></p>
<p><strong><strong>input:</strong></strong></p>
<pre>6 9<br>10 20 20 10 10 20<br></pre>
<p><strong>output:</strong></p>
<pre>36<br></pre>
<p><em>We are not allowed to put a cube of size 20 onto a cube of size  10. There are six ways to order the cubes of size 10, and six ways to  order the cubes of size 20.</em></p>