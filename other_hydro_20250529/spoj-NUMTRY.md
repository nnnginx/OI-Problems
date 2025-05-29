<p>f(n) and g(n) are two functions defined as following :</p>
<p>f(n) = <span style="font-size: small;">กว</span>( p<sub>i</sub><sup>2e<sub>i</sub>+1</sup>+1 ), where p<sub>i</sub> is prime factor of n and e<sub>i</sub> is highest power of p<sub>i</sub> in n.</p>
<p>g(n) = <span style="font-size: small;">ฆฒ</span>( n/gcd(n,i) ); 1 &lt;= i&nbsp; &lt;= n</p>
<p>For a given value of n, you have to compute [f(n)/g(n)] % 1000000007.</p>
<h3>Input</h3>
<p>First line has T ( &lt;= 10000 ), next T lines has 2 &lt;= n &lt;= 10^12.</p>
<h3>Output</h3>
<p>[f(n)/g(n)] % 1000000007 for each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2<br>4

<strong>Output:</strong><br>3<br>3 <br><br></pre>
<p><strong>Warning:</strong> Test cases aren't random. Test files consist of large  primes, strong  pseudo primes, Carmichael numbers, squares of primes,  product of large  primes, worst possible test cases for fermat, miller  rabin and other  primality testing algorithms.</p>
<p><strong>Note</strong>: You may try the<a href="../NUMTRYE"> tutorial version </a>( same test files, 5s-100s time limit ).<strong>&nbsp;</strong></p>
<p>&nbsp;</p>