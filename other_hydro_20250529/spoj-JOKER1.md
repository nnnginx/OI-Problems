<p><strong>"</strong><strong>Do you know, why I use a knife? Guns are too quick. You can't savor all the little emotions. You see, in their last moments, people show you who they really are. So in a way, I know your friends better than you ever did. Would you like to know which of them were cowards?"</strong></p>

<p>Joker has many knifes, and he wants to assign a distinct integer to each knife so he can easily identify them. The i-th knife can have an integer between 1 and maxNumber[i], inclusive.</p>
<p>Return the number of ways he can assign numbers to his knifes, modulo 1,000,000,007. If it's impossible to assign distinct integers to the knifes, print 0.</p>

<h3>Input</h3>
<p>The first line contains the number of test cases T (1 &lt;= T &lt;= 666)</p>
<p>Each test case has 2 lines - 1st line denotes number of knifes N (1 &lt;= N &lt;= 66) Joker has and the 2nd line denotes the numbers {maxNumber[0]....maxNumber[N-1]} Joker has.</p>
<p>1 &lt;= maxNumber[i] &lt;= 3000</p>

<h3>Output</h3>
<p>Print the number of ways Joker can assign numbers to his knifes, modulo 1,000,000,007. If it's impossible to assign distinct integers to the knifes, print 0. In last line print the string "<tt>KILL BATMAN</tt>".
Don't print any extra spaces.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
1
7
2
5 8
3
2 1 2

<strong>Output:</strong>
7
35
0
KILL BATMAN</pre>

<h3>Explanation</h3>
<ul>
  <li>Test case 1 : Joker can assign any number between 1 and 7, inclusive, to the only knife.</li>
  <li>Test case 2 : Joker wants you too think !</li>
  <li>Test case 3 : (1,1,1) (1,1,2) (2,1,1) (2,1,2) are the possible combinations . As the numbering of knifes is not unique so the output is 0.</li>
</ul>