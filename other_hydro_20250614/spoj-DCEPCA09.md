<p>Everyone knows how to find mean, median and mode of an array of numbers. For people who don¡¯t know this, here is the description:<br> Mean is the arithmetic average of a set of values.<br> Median of a finite list of numbers can be found by arranging all the observations from lowest value to highest value and picking the middle one. If there is an even number of observations, then there is no single middle value; the median is then usually defined to be the mean of the two middle values.<br> The mode is the value that appears most often in a set of data. If more than one number is applicable to be the mode, select the highest value number amongst them as the mode.</p>
<p>The problem is just to find these 3 values. Given an array of numbers and two indices i and j , find the mean , median and mode of elements in the interval i to j including numbers at indices i and j. Note that i and j are 0 index based.</p>
<h3>Constraints</h3>
<p>2 &lt;= N &lt;= 10000<br> 1 &lt;= Q &lt;= 10000<br> 0 &lt;= A[i] &lt;= 10^8<br> 0 &lt;= i &lt; N<br> i &lt;= j &lt; N</p>
<h3>Input</h3>
<p>First line contains N which is the total number of numbers in the array. The next line contains N numbers A[i] which are the elements of the array. Next line contains a number Q which defines the total number of queries we are making for the interval i to j. It is followed by Q lines each containing 2 numbers i and j which denotes the indices to be queried for.</p>
<h3>Output</h3>
<p>Print Q lines each containing 3 numbers Mean, Median and Mode respectively. If the answer for any case comes to be a floating point, then take the integer part of the number as the answer.<br> For example: if mean, median and mode comes up to be 6.44 7.8 9 then the final answer is 6 7 9.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>6 5 3 7 7<br>2<br>1 2<br>0 4<br><br>&nbsp;<strong>Output:</strong>
4 4 5<br>5 6 7</pre>