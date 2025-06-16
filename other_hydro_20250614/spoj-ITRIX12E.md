<h3>R - Numbers</h3>
<p>R-numbers are numbers which have the property that they do not have the digit '0 ' and sum of every two adjacent digits of the number is prime. 123 is a R-number because 1+2 =3 and 2+3 =5 and 3 , 5 are primes.</p>
<p>How many R-numbers can be formed with atmost length N?</p>
<p>i.e R-numbers of length 1 + R-numbers of length 2 + R-numbers of length 3+....... R-numbers of length N</p>
<p>Length of a number = Number of digits in the number</p>
<p>Only four single digit numbers are R-numbers which are nothing but single digit primes 2,3,5,7</p>

<h3>Input Specification</h3>
<p>
The first line of the input file contains T which denotes the number of Test cases.The next T lines contain an integer N &lt;= 10^9
</p>

<h3>Output Specification</h3>
<p>
Print the numbers of R-numbers modulo 1000000007. [10^9+7];
</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
1
2

<strong>Sample Output:</strong>
4
33</pre>