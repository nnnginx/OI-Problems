<p>In the field of Cryptography, prime numbers play an important role. We are interested in a scheme called "Diffie-Hellman" key exchange which allows two communicating parties to exchange a secret key. This method requires a prime number <b>p</b> and <b>r</b> which is a primitive root of p to be publicly known. For a prime number p, r is a primitive root if and only if it's exponents r, r<sup>2</sup>, r<sup>3</sup>, ... , r<sup>p-1</sup>  are distinct (mod p).
</p><p>
Cryptography Experts Group (CEG) is trying to develop such a system. They want to have a list of prime numbers and their primitive roots. You are going to write a program to help them. Given a prime number p and another integer r &lt; p , you need to tell whether r is a primitive root of p.

</p><h3 align="center">Input</h3>
<p>There will be multiple test cases. Each test case starts with two integers <b>p</b> ( p &lt; 2 <sup> 31 </sup> ) and <b>n</b> (1 ¡Ü n ¡Ü 100 ) separated by a space on a single line. p is the prime number we want to use and n is the number of candidates we need to check. Then n lines follow each containing a single integer to check. An empty line follows each test case and the end of test cases is indicated by p=0 and n=0 and it should not be processed. The number of test cases is atmost 60.</p>

<h3 align="center">Output</h3>
<p>For each test case print "YES"  (quotes for clarity) if r is a primitive root of p and "NO" (again quotes for clarity) otherwise.</p>

<h3 align="center">Example</h3>

<pre><b>Input:</b>
5 2
3
4

7 2
3
4

0 0


<b>Output:</b>
YES
NO
YES
NO
</pre>


<h3 align="center">Explanation</h3>
<p> In the first test case  3<sup>1</sup>, 3<sup>2 </sup>, 3<sup>3</sup> and 3<sup>4</sup> are respectively 3, 4, 2 and 1 (mod 5). So, 3 is a primitive root of 5. </p>
<p>4<sup>1</sup>, 4<sup>2</sup> , 4<sup>3</sup> and 4<sup>4</sup> are respectively 4, 1, 4 and 1 respectively. So, 4 is not a primitive root of 5. </p>