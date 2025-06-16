Walter is a high school chemistry teacher. After being diagnosed with stage 3A, inoperable lung cancer, Walter is devastated. Realizing he does not have much time left, a desperate Walter resorts to cooking crystal methamphetamine, in order to provide for his treatment and family. And guess what, he mixes up with some really horrible people in the process.
<br><br>

The worst of them is Heisenburg, a badass physicist and the ultimate drug lord. Walter needs Heisenburg¡¯s active support to distribute the methamphetamine he produces. Alas, Heisenburg is a cautious man. Heisenburg is initially skeptical about Walter, and decides to give the following problem to Walter in order to prove his worth.
<br><br>

<strong>w(n)</strong> is defined to be the number of distinct prime factors of <strong>n</strong>, for example:
<br><br>
<strong>w(1) = 0, w(2) = 1, w(3) = 1, w(4) = 1, w(5) = 1, w(6) = 2, w(30) = 3</strong>
<br><br>

<strong>f(n, k) = ¡Æ k<sup>w(i)</sup></strong> where <strong>1 ¡Ü i ¡Ü n</strong>
<br><br>
For instance, <strong>f(6,2) = 2<sup>w(1)</sup> + 2<sup>w(2)</sup> + 2<sup>w(3)</sup> + 2<sup>w(4)</sup> + 2<sup>w(5)</sup> + 2<sup>w(6)</sup> = 13</strong>
<br><br>

Given <strong>n</strong> and <strong>k</strong>, calculate <strong>f(n, k)</strong>.
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>t</strong>, denoting the number of test cases. Each of the next <strong>t</strong> lines contains two integers, <strong>n</strong> and <strong>k</strong>, separated by a single space. Sum of <strong>n</strong> will not exceed <strong>10<sup>11</sup></strong> in an input file.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü t ¡Ü 100</li></strong>
<strong><li>1 ¡Ü n ¡Ü 10<sup>11</sup></li></strong>
<strong><li>1 ¡Ü k ¡Ü 10</li></strong>
<strong><li>1 ¡Ü ¡Æn ¡Ü 10<sup>11</sup></li></strong>

<h3>Output</h3>
For each case, output a line of the format <strong>Case X: Y</strong>, where <strong>X</strong> is the case number, starting from <strong>1</strong>, and <strong>Y</strong> is the required answer. You can safely assume that the answer will fit in a <strong>signed 64 bit integer</strong>.

<h3>Sample Input</h3>
<pre>10
1 1
2 2
3 3
4 4
5 5
6 6
7 7
8 8
9 9
10 10
</pre>

<h3>Sample Output</h3>
<pre>Case 1: 1
Case 2: 3
Case 3: 7
Case 4: 13
Case 5: 21
Case 6: 61
Case 7: 85
Case 8: 113
Case 9: 145
Case 10: 271
</pre>

<br><br>