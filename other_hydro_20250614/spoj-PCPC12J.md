<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Amr started to learn division. So he gave a list of numbers to his friend and asked him to find all the divisors of each number in the given list. Now Amr has a new list of numbers containing all divisors of his original list.&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">As Amr loves playing with numbers, he now thinks about the repeated numbers in the new list of divisors. However this time Amr is interested in the luckiest divisor!</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Lucky divisor is defined by Amr as follows: a divisor D is lucky if D divides f, where f is the frequency of this number D in the new list. Obviously f must be greater than zero.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">The luckiest divisor is the divisor D that divides f where f is the maximum and D is the smallest one.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Since Amr is too lazy to write a program that solves this problem, he decided to submit it to the PCPC chief judge to put it as a problem for the teams to write a solution to it. Can you write this program for Amr?</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Input Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">The first line contains a positive integer t &lt;= 100, then follow t test cases. Each test case start with a line containing a single positive integer n &lt;= 10000 number of divisors in Amr¡¯s new list, then follows n positive integers a1, ai, ¡­an (ai&lt;= 100).</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Output Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Your code should print an integer for each test case representing the luckiest divisor or -1 if there is no lucky divisor.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2 2 3 3 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">7</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2 2 2 2 3 3 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2</span></div>
<p>&nbsp;</p>
<p><span style="font-size: small;">Amr started to learn division. So he gave a list of numbers to his friend and asked him to find all the divisors of each number in the given list. Now Amr has a new list of numbers containing all divisors of his original list.&nbsp;</span></p>
<p><span style="font-size: small;">As Amr loves playing with numbers, he now thinks about the repeated numbers in the new list of divisors. However this time Amr is interested in the luckiest divisor!</span></p>
<p><span style="font-size: small;">Lucky divisor is defined by Amr as follows: a divisor D is lucky if D divides f, where f is the frequency of this number D in the new list. Obviously f must be greater than zero.</span></p>
<p><span style="font-size: small;">The luckiest divisor is the divisor D that divides f where f is the maximum and D is the smallest one.</span></p>
<p><span style="font-size: small;">Since Amr is too lazy to write a program that solves this problem, he decided to submit it to the PCPC chief judge to put it as a problem for the teams to write a solution to it. Can you write this program for Amr?</span></p>
<p><span style="font-size: small;"><strong>Input Specification</strong></span></p>
<p><span style="font-size: small;">The first line contains a positive integer t &lt;= 100, then follow t test cases. Each test case start with a line containing a single positive integer n &lt;= 10000 number of divisors in Amr¡¯s new list, then follows n positive integers a1, ai, ¡­an (ai&lt;= 100).</span></p>
<p><span style="font-size: small;"><strong>Output Specification</strong></span></p>
<p><span style="font-size: small;">Your code should print an integer for each test case representing the luckiest divisor or -1 if there is no lucky divisor.</span></p>
<p><span style="font-size: small;"><strong>Sample Input</strong></span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;">2 2 3 3 3</span></p>
<p><span style="font-size: small;">7</span></p>
<p><span style="font-size: small;">2 2 2 2 3 3 3</span></p>
<p><strong><span style="font-size: small;">Sample Output</span></strong></p>
<p><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">2</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>