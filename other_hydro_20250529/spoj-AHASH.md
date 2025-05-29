Given a base <strong>B</strong> and a modulus <strong>M</strong>, the polynomial hash of a string <strong>S</strong>, consisting of only lowercase letters <strong>(a-z)</strong> is defined as below:

<br><br>

<pre>int Hash(string S, int B, int M){
     long long H = 0;
     for (int i = 0; i &lt; S.length(); i++){
           H = (H * B + S[i] - 'a' + 1) % M;
     }
     return H;
}
</pre>
<br><br>

In other words, first the letters of the string are replaced by numbers (equivalent to their position, <strong>'a'</strong> gets mapped to <strong>1</strong>, <strong>'b'</strong> to <strong>2</strong>, ... and <strong>'z'</strong> to <strong>26</strong>). This is then considered to be a number in base <strong>B</strong> (rightmost number is the least significant digit), and the value of this number in <strong>base 10</strong> modulo <strong>M</strong> is called the polynomial hash of the string.
<br><br>

Limak the bear loves to hack other contestants in Codeforces. After the recent educational round, he came to know that his friend Swistak used the polynomial hash function stated above to solve the hardest problem! And believe it or not, he was the only one to solve that problem! Limak is so angry, how can Swistak solve a problem which Limak himself couldn't solve? And worst of all, Swistak used hashing to solve that problem! Limak believes people who uses hashing have no real skill, getting <i>Accepted</i> just implies getting lucky, nothing more!
<br><br>

Later that night, Limak realized that he can hack the solution if he is able to solve the following problem efficiently. Limak felt triumphant, he will teach Swistak and that stupid hash function of his a lesson! But Limak is just a little bear, he is not very good at solving problems. Please help Limak solve the following problem so that he can hack Swistak's solution.
<br><br>

Limak will give you a string <strong>S</strong> of length <strong>N</strong>, consisting of only lowercase letters, a base <strong>B</strong> and a modulus <strong>M</strong>. Your task is to find another string <strong>T</strong>, satisfying all of the following constraints:
<br><br>

<li>Length of <strong>T</strong> is exactly <strong>N</strong></li>
<li><strong>T</strong> consists of only lowercase letters <strong>(a-z)</strong></li>
<li><strong>T</strong> and <strong>S</strong> are two different strings</li>
<li><strong>T</strong> and <strong>S</strong> have the same hash, i.e. <strong>Hash(S, B, M) = Hash(T, B, M)</strong></li>

<br><br>


<h3>Input</h3>
The first line contains <strong>Q</strong>, denoting the number of test cases. Each test case consists of two lines. The first line of each case contains three integers, <strong>N, B, M</strong>. The next line contains the string <strong>S</strong> of length <strong>N</strong>, consisting of only lowercase letters.

<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü Q ¡Ü 30</li></strong>
<strong><li>10<sup>5</sup> ¡Ü N ¡Ü 10<sup>6</sup></li></strong>
<strong><li>10<sup>5</sup> ¡Ü B &lt; 2<sup>31</sup></li></strong>
<strong><li>10<sup>5</sup> ¡Ü M &lt; 2<sup>31</sup></li></strong>
<strong></strong><li><strong>Si ¡Ê {a-z}</strong>
<strong></strong></li><li><strong>B ¡Ù M and both B and M are prime numbers</strong></li>

<h3>Output</h3>
For each test case, output the string <strong>T</strong> in a single line. It is guaranteed that such a string will always exist for the given constraints. If there are many solutions, you can output any of them.


<h3>Sample Input</h3>
<pre>1
38 666666667 1000000009
bbababbbbbbbaabaababaabbababbababababb


</pre>

<h3>Sample Output</h3>
<pre>hisotomeseemslikeanotoriouscoincidence

</pre>

<h3>Note</h3>
<strong>The sample input contains a string of length 38 only for demonstration and clarity. There will be no such cases in the judge data, every case will strictly satisfy the constraints mentioned above.</strong>

<br><br>

<h3>Challenge</h3>
You might also enjoy:
<br><br>
<a href="https://www.spoj.com/problems/AHASH2/">Anti Hash II</a>