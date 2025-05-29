<pre><br><p style="font-family: 'Times New Roman'; font-size: medium;">Geometric progression(GP) is a set in which the ratio of 2 consecutive numbers is same. for eg, 1,2,4,8,16.... In this the ratio of the numbers is 2.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">The task here is very simple indeed.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">You will be given the 3rd term , 3rd last term and the sum of the series. You need print length of the series &amp; the series.</p>
<h3 style="font-family: 'Times New Roman';">Input</h3>
<p style="font-family: 'Times New Roman'; font-size: medium;">First line will contain a number indicating the number of test cases.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Each of the following t lines will have 3 number '3term' ,'3Lastterm' and 'sum'</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">3term&nbsp; - is the 3rd term in of the series and</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">3Lastterm&nbsp; - is the 3rd term in of the series and</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">sum - is the sum of the series.</p>
<h3 style="font-family: 'Times New Roman';">Output</h3>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each input of the test case, you need to print 2 lines.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">fist line should have 1 value- number of terms in the series.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">2nd line of the output should print the series numbers separated by single space</p>
<h3 style="font-family: 'Times New Roman';">Example</h3>
<pre><strong>Input:</strong>
<br>1<br>4 64 511<br><br>&nbsp;<strong>Output:</strong>
<br>9<br>1 2 4 8 16 32 64 128 256<br><strong><br><br>NOTE </strong>-<br>All the values will be in the range [0, 2^64] inclusive<br>The series will have at least 6 elements.<br>number of test cases &lt;=100.<br>The Ratio in all the cases will be an integer. (Thanks Mitch for pointing this out)<br>All the numbers will fit in 64 bits(long long in C)</pre>
</pre>