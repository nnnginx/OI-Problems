<p><span style="white-space: normal;">&nbsp;</span></p>
<p>Palindromes are numbers that read the same forwards and backwards. Your friend Percy recently became interested in a special kind of palindrome that he calls a&nbsp;<em>Nested Palindrome</em>. A&nbsp;<em>Nested Palindrome</em>&nbsp;meets three conditions:</p>
<ul>
<li>The number is a palindrome.</li>
<li>Split the number in the middle. The first half of the digits of the number is also a <em>Nested Palindrome</em>. If the number has an odd number of digits, don¡¯t consider the middle digit as part of the first half.</li>
<li>No two adjacent digits are the same.</li>
</ul>
<p>Percy says that he has written a <em>Nested Palindrome</em> with no leading zeros on a slip of paper. Next, Percy says that he has erased some of the digits in the number and replaced those digits with question marks. He asks you to think about all possible numbers, in increasing order, that can fill those digits and could possibly form the number Percy wrote. Of course, Percy may not be telling the truth about having written a <em>Nested Palindrome</em> in the first place.</p>
<p>Percy tells you that the number he wrote is the <strong>k</strong>th number of this potentially large list. Your task is to find that <strong>k</strong>th number.</p>
<h3><span style="font-size: 1.17em;">Input</span></h3>
<p><span style="font-size: small;">There will be several test cases in the input. Each test case will consist of two lines. The first line will contain an integer&nbsp;<strong>k</strong>&nbsp;(1¡Ü<strong>k</strong>¡Ü10<sup>18</sup>), which is the position in the ordered list you must find. The second line contains a string of length 1 to 10,000, consisting only of digits (¡®0¡¯ to ¡®9¡¯) and question marks (¡®?¡¯). Input is terminated by a line with a single&nbsp;<strong>0</strong>.</span></p>
<h3><span style="font-size: 1.17em;">Output</span></h3>
<p><span style="font-size: small;">For each test case, output the&nbsp;<em>Nested Palindrome&nbsp;</em>that Percy is looking for. If that number does not exist, or if the string cannot form a&nbsp;<em>Nested Palindrome</em>, output&nbsp;<strong>-1</strong>. Output no spaces, and do not separate answers with blank lines.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 <br>1?1 <br>1 <br>?3? <br>1 <br>?1? <br>55 <br>??? <br>55 <br>1?1 <br>3 <br>0?0 <br>0

<strong>Output:</strong>
101 <br>131 <br>212 <br>707 <br>-1 <br>-1&nbsp;</pre>