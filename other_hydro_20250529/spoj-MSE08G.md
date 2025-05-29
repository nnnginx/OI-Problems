<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MSE08G/en/">English</a></td> 
<td width="50%"><a href="/problems/MSE08G/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
 
John has recently arrived in Bucharest for the South Eastern 
European Regional Contest. John is famous for his theory of lucky 
numbers. That¡¯s why all the contestants and spectators are very happy. 
According to that theory  4 and  7 are lucky digits, and all the 
other digits are not lucky. A lucky number is a number that contains 
only lucky digits in decimal notation. A very lucky number is a number 
that can be expressed as a product of several lucky numbers. A lucky 
number by itself is considered to be very lucky. For  example, numbers 
47, 49, 112 are very lucky. </p><p>
Your task is to calculate the number of very lucky numbers that are 
not less than A and not greater than B. Of course, numbers A and B are 
given by John. </p><p>
 
 
</p><h3>Input</h3>
<p></p><p>
The first line of the input contains a single integer T ¨C a number 
of test cases. Each of the next T lines contains two integers separated 
by a single space ¨C A and B. 
</p><p>
</p><h3>Output</h3>
<p></p><p>
Output must contain T lines ¨C answers for the test cases. 
Constrains: </p><p>
1 ¡Ü T ¡Ü 7777, </p><p>
1 ¡Ü A ¡Ü B ¡Ü 1000000000000 (10^12).  </p><p>
 
 
</p><h3>Sample</h3>
<pre>Input :
4 
1 2 
88 99 
112 112 
1 100 
Ouput: 
0 
0 
1 
10 

 
Hint: 
Very lucky numbers for the last case are 4, 7, 16, 28, 44, 47, 49, 64, 74 and 77. 
</pre>