<p>In this problem you have to calculate the determinant of an N x N matrix whose entries are given by <b>m[i][j] = gcd(i,j)<sup>k</sup></b>, 1 ¡Ü i,j ¡Ü N.<br><br>
Here gcd(i,j) denotes the greatest common divisor of i and j.<br><br>
As the determinant D can grow very large, you have to print D%1000003.

</p><h3>Input</h3>
<p>First line of input consists of a single integer containing the number of test cases T ( equal to around 20), each of the following T lines contain two integers N and k where N is the size of the matrix and k is the exponent.<br>
1 ¡Ü N ¡Ü 1000000<br>
1 ¡Ü k ¡Ü 10<sup>9</sup><br>

</p><h3>Output</h3>
<p>One line corresponding to each test case containing the determinant modulo 1000003 for the corresponding test case.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
4 2
2 4
4 3


<b>Output:</b>
288
15
10192
</pre>

<b>Note</b>: You may want to solve <a href="https://www.spoj.com/problems/DETER">DETER</a> first, in case you havent already solved it.