<p><span style="font-size: small;"> It's the year 4224 and Giant Machine Corporation has started working on it¡¯s   42nd Generation Robots. These robots are designed to have peculiar   specifications. </span></p>
<p><span style="font-size: small;"> The company has <strong>N</strong> different parts (numbered from <strong>1 to N</strong>), each of which impart   a very specific property to the robot. The formation of a single robot <strong>R</strong> consists of <strong>M</strong> steps. At the <strong>i<sup>th</sup></strong> step, one of the <strong>N</strong> parts is chosen and added   to the current robot. After the <strong>M<sup>th</sup></strong> step, the robot is ready.   Let <strong>num(i, j)</strong> be the count of part number <strong>j</strong> till the <strong>i<sup>th</sup></strong> step used for making   the robot <strong>R</strong>.</span></p>
<p><span style="font-size: small;"> The 41st Generation Robots were found to be defective in the sense that one of   their properties overshadowed their other properties significantly. Hence, for   the 42nd Generation, it was decided that for any robot <strong>R</strong>, <strong>|num(i, j) ¨C num(i,   k)| ¡Ü 2</strong> for every <strong>1 ¡Ü i ¡Ü M</strong> and for every pair of <strong>j, k </strong>where <strong>1 ¡Ü j,k ¡Ü N</strong> .</span></p>
<p><span style="font-size: small;">Now, the Giant Machine Corporation is interested to know the number of   different 42nd Generation Robots that they can make which satisfy the above   criteria and hence they have hired you for the task. Since, this number can be   very large, output the result modulo <strong>10^9 + 7</strong>.</span></p>
<p><span style="font-size: small;"><strong>Note</strong> : Two robots <strong>R1</strong> and <strong>R2</strong> are considered different, if a different part is   used in any of the corresponding <strong>i</strong> steps out of <strong>M</strong> steps. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> The first line starts with an integer <strong>T</strong>, denoting the number of test cases. <strong>T</strong> lines follow with each line consisting of two space separated integers <strong>M</strong> and   <strong>N</strong>. </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> For each test case, print in a single line the required number. </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 ¡Ü T ¡Ü 20<br> 1 ¡Ü N ¡Ü 50<br> 1 ¡Ü M ¡Ü 10^18<br></strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">3
1 1
2 2
3 2</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">1
4
6</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Vivek Hamirwasia</strong></span></p>