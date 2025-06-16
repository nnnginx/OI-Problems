Are you familiar with polynomial hashing? If you are not, all the better! You don¡¯t need to know what polynomial hashing is, the world is better off without it. I hate polynomial hashing so much that I found a new way to hash strings. It is called the <i>Faketorial Hashing</i>.
<br><br>

First, let¡¯s define a function, <i>ord(ch)</i> = the position of <i>ch</i> in the alphabet + 1, where <i>ch</i> can be any lowercase letter. So, <i>ord(a) = 2,  ord(b) = 3,  ord(c) = 4, ¡­  ord(z) = 27</i>.
<br><br>
Let <i>fact(x)</i> be <i>x!</i> or the factorial of x. A few examples, <i>fact(1) = 1, fact(2) = 2, fact(3) = 6, fact(4) = 24, fact(5) = 120</i>, etc.
Given a string <strong>S</strong> of length <strong>N</strong>, consisting of lowercase letters only, the <i>Faketorial Hashing</i> of S, is defined as below:
<br><br>
<strong>fake_hash(S) = fact(ord(S[0])) ¡Á fact(ord(S[1])) ¡Á fact(ord(S[2])) ¡Á ¡­¡­ ¡Á fact(ord(S[N - 1]))</strong>
<br><br>
In other words, it is the product of the factorial of the <strong>ord()</strong> value of all the characters in <strong>S</strong> (That¡¯s right, no modulus! Unlike the lame polynomial hashing).
Not only that we have a new hashing mechanism in place, but we would also like to crack this now. Given a string <strong>S<sub>1</sub></strong> consisting of lowercase letters only, your task is to find a different string <strong>S<sub>2</sub></strong> consisting of lowercase letters, such that, <strong>fake_hash(S<sub>1</sub>) = fake_hash(S<sub>2</sub>)</strong> and <strong>S<sub>1</sub> ¡Ù S<sub>2</sub></strong>.
<br><br>
If there are multiple possible choices for <strong>S<sub>2</sub></strong>, you need to find the <strong>lexicographically smallest</strong> one, or output the word <i>¡°Impossible¡±</i> without quotes, if it is not possible to find such a string.
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases.  Each test case contains the string <strong>S<sub>1</sub></strong> consisting of lowercase letters (a-z) only.

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 3000</li></strong>
<strong><li>1 ¡Ü <strong>|S<sub>1</sub>|</strong> ¡Ü 30</li></strong>

<br><br>
Except for the sample, the following constraints will hold:
<strong><li>1 ¡Ü |S<sub>1</sub>| ¡Ü 5, for 90% of the test cases </li></strong>
<strong><li>1 ¡Ü |S<sub>1</sub>| ¡Ü 15, for 99% of the test cases </li></strong>

<h3>Output</h3>
For each test case, output the case number followed by the required output. Please refer to the sample input/output section for the precise format.

<h3>Example</h3>
<pre><b>Input:</b>
10
tourist
petr
mnbvmar
bmerry
xellos
sevenkplus
dragoon
zzz
snapdragon
zosovoghisktwnopqrstuvwxyzoos


<b>Output:</b>
Case 1: aaaaabbdnstttu
Case 2: aqst
Case 3: abmmnrv
Case 4: aaabbnrry
Case 5: aaaaaaadddlnuz
Case 6: aaaaaaabbddddnquuuz
Case 7: aaaaaaaaaaaaabdnnnt
Case 8: Impossible
Case 9: aaaaaaaaaabdnnnpst
Case 10: aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaffffjnnnnqqttttuuuuxxzzzzzz

</pre>