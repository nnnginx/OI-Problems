<p>It is the 10-th ACM Egyptian National Programming Contest and Mostafa S., the chief judge, started to prepare for the problem set. In previous years, a chief judge used to ask problems�� setters to use his public key to encrypt the data so that they keep everything related to the problems secured. Unfortunately, the RSA algorithm was broken 2 weeks ago and Mostafa decided to invent a temporary algorithm till someone finds a new robust approach for encrypting/decrypting&nbsp; plaintext. After finding the algorithm, Mostafa met the judges and described the new encryption algorithm for them and gave them an equation to generate a key which the algorithm depends on. The key is generated through the following equation:</p>
<p align="center"><strong>SKEY = (M * SUM [1 / A^K (from k = 0 to k = N)] ) % P</strong><strong> <br></strong></p>
<p>A, N and P are integers and P is a prime number that is co-prime with A (e.g. gcd(A, P) = 1). Furthermore M is a very large number (millions of digits) generated to be divisible by    . <strong>For example</strong> given: A = 3, N = 2, P =&nbsp; 7&nbsp; and M = 18, then the skey value is:</p>
<p>&nbsp;(18 * (1/1 + 1/3 + 1/9)&nbsp; ) % 7 = 26 % 7 = 5.</p>
<p>&nbsp;</p>
<p>Unfortunately, sending extremely large numbers for M in the emails between judges is impractical. Luckily, a property of the modulus operator is: (A*B)%X = (A%X * B%X) %X.</p>
<p>Hence, we still can find our way to evaluate the skey by replacing M with M%P.</p>
<p>&nbsp;</p>
<p>Given A, N, P, M%P, kindly help the chief judge with writing a code to compute the SKey.</p>
<p><strong>Input Specification:</strong></p>
<p>The first line of input contains an integer T that represents the number of test cases, then follow T lines each contains only four integer numbers A, N, P where 1 �� A �� 2147483647, 0 �� N �� 2147483647, 2 �� P �� 2147483647 and 0 �� M%P &lt; P.</p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, output a single line of output in the form <strong>��Case K: SKey��</strong> where K is the number of the test case and Skey is as defined in the problem statement. Check sample below for the format.</p>
<p><strong>Sample input:</strong></p>
<p>1</p>
<p>3 2 7 4</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: 5</p>