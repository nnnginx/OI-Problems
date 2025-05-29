<p>Given a list of n d-digit numbers, choose the smallest subset from the list that covers all the digits [0-9].&nbsp;</p>
<h3>Input</h3>
<p>First line contains a positive integer T representing number of testcases.</p>
<p>Next line contains two numbers n and d, where n is the size of the list and d is number of digits in each number.</p>
<p>Next n lines follow each containing a d digit number made from [0-9]</p>
<p>1 ¡Ü t ¡Ü 100</p>
<p>1 ¡Ü n ¡Ü 1000</p>
<p>1 ¡Ü d ¡Ü 1000</p>
<h3>Output</h3>
<p>Output the length of the smallest subset that covers all digits [0-9]. Return -1 if not possible.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>
2<br>
4 5<br>
01234<br>
56789<br>
01456<br>
13452<br>
4 5<br>
11234<br>
56789<br>
01456<br>
13452</pre>
<pre><strong>Output:</strong><br>
2<br>
3</pre>
<pre><strong>Explanation:</strong><br>
Smallest set will be {01234,56789}<br>
Smallest set will be {11234,56789,01456}
</pre>