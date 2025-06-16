<p>A palindrome is a symmetrical string, that is, a string read identically from left to right&nbsp;as well as from right to left. You are to write a program which, given a string,&nbsp;determines the minimal number of characters to be inserted into the string in order to&nbsp;obtain a palindrome.&nbsp;As an example, by inserting 2 characters, the string "Ab3bd" can be transformed into&nbsp;a palindrome ("dAb3bAd" or "Adb3bdA"). However, inserting fewer than 2&nbsp;characters does not produce a palindrome.</p>
<h3>Input</h3>
<p>The first line contains one integer: the length of&nbsp;the input string N, 3¡ÜN¡Ü5000. The second line contains one string with length N. The&nbsp;string is formed from uppercase letters from ¡®A¡¯ to ¡®Z¡¯, lowercase letters from ¡®a¡¯ to&nbsp;¡®z¡¯ and digits from ¡®0¡¯ to ¡®9¡¯. Uppercase and lowercase letters are to be considered&nbsp;distinct.</p>
<h3>Output</h3>
<p>The first line contains one integer, which is the&nbsp;desired minimal number.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
Ab3bd

<strong>Output:</strong>
2</pre>