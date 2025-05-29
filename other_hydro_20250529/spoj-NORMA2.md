<p>Mirko got an array of integers for his birthday from his grandmother Norma. As any other kid, he was hoping for some money, but got an array. Luckily, in his town there is a pawn shop that buys up arrays. The cost of an array of integers is <b>min</b> * <b>max</b> * <b>L</b> kunas, where <b>min</b> is the minimal integer in the array, <b>max</b> is the maximal and <b>L</b> is the array length. Mirko is going to sell a subsequence of consecutive numbers from his array. He calculated the average price of all such subsequences.</p>
<p>In order to check his result, he wants you to do the same. He will be pleased with only the last 9 digits of the sum of all prices, so you don¡¯t need to bother with large and real numbers.</p>

<h3>Input</h3>
<p>The first line of input contains an integer N (1 ¡Ü N ¡Ü 500 000).</p>
<p>Each of the following N lines contains a member of Mirko¡¯s array. The members of the array will be integers from the interval [1, 10<sup>8</sup>].</p>

<h3>Output</h3>
<p>The first and only line of output must contain an integer, the last 9 digits of the required sum from the task. <b>You don¡¯t need to output</b> the leading zeroes of that 9-digit integer.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1<br>3&nbsp;</pre>
<pre><strong>Output:</strong>
16</pre>
<pre><strong>Input:<br></strong>4<br>2<br>4<br>1<br>4</pre>
<pre><strong>Output:<br></strong>109</pre>
<pre><strong>Input:<br></strong>6<br>8<br>1<br>3<br>9<br>7<br>4</pre>
<pre><strong>Output:<br></strong>1042</pre>