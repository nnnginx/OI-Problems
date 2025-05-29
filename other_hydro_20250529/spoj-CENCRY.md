<p>Marko is going to write a secret letter to a friend. He thought it is better to encrypt letter so that no other person can read it. After long thought he came up with an encryption scheme which was lame but he thought it will work anyways.<br><br>To encrypt a text he first wrote two infinite strings of characters first string consists only of vowels and second string consists of consonants only.</p>
<p>aeiouaeiouaeiouaeiouaeiou....................<br>bcdfghjklmnpqrstvwxyzbcdfghjklmnpqrstvwxyz...<br>&nbsp;<br>Following is the scheme for encryption :<br>1. let c be any character to be encrypted.<br>2. let k be the count of number of times c character occured in text to be encrypted till now.<br>3. first find which of two infinite string contains that character.<br>4. then look for kth occurence of that character in that string.<br>5. replace charcter c by corresponding character in second string.<br><br>For example encrypted text of "baax" will be "abho".</p>
<h3>Input</h3>
<p>First line of input will contains t, number of test cases. Then t test case follows each test case in a line. Each test case will be a string of small latin alphabets. Length of string will be less than 5*10^4</p>
<h3>Output</h3>
<p>For each test case print encrpyted text.</p>
<p><strong>Sample :</strong></p>
<p><strong>Input:</strong></p>
<p>2<br>baax<br>aaa</p>
<p><strong>Output:</strong></p>
<p>abho<br>bhn</p>