<p style="text-align: left;">For a string of n bits x1,x2,x3,...,Xn the adjacent bit count of the string (AdjBC(x)) is given by</p>
<p style="text-align: center;"><br>X1*X2 + X2*X3 + X3*X4 + ... + Xn-1 * Xn</p>
<p><br>which counts the number of times a 1 bit is adjacent to another 1 bit. For example:<br>AdjBC(011101101) = 3<br>AdjBC(111101101) = 4<br>AdjBC(010101010) = 0</p>
<p>Write a program which takes as input integers n and k and returns the number of bit strings x of n bits (out of 2ⁿ) that satisfy AdjBC(x) = k. For example, for 5 bit strings, there are 6 ways of getting AdjBC(x) = 2:<br>11100, 01110, 00111, 10111, 11101, 11011</p>
<h3>Input</h3>
<p>The first line of input contains a single integer P, (1 ≤ P ≤ 1000), which is the number of data sets that follow. Each data set is a single line that contains the data set number, followed by a space, followed by a decimal integer giving the number (n) of bits in the bit strings, followed by a single space, followed by a decimal integer (k) giving the desired adjacent bit count. The number of bits (n) will not be greater than 100 and the parameters n and k will be chosen so that the result will fit in a signed 32-bit integer.</p>
<h3>Output</h3>
<p>For each data set there is one line of output. It contains the data set number followed by a single space, followed by the number of n-bit strings with adjacent bit count equal to k.</p>
<h3>Example</h3>
<pre><span style="color: #ff0000;"><strong>Input:</strong>
</span>10<br>1 5 2<br>2 20 8<br>3 30 17<br>4 40 24<br>5 50 37<br>6 60 52<br>7 70 59<br>8 80 73<br>9 90 84<br>10 100 90
<strong></strong></pre>
<pre><strong><span style="color: #ff0000;">Output:</span></strong>
1 6<br>2 63426<br>3 1861225<br>4 168212501<br>5 44874764<br>6 160916<br>7 22937308<br>8 99167<br>9 15476<br>10 23076518
</pre>