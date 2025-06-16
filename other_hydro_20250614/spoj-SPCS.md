<p>Gopu loves palindromes. A palindrome is a string which is same even when it is reversed. eg. aba, a, abba are palindromes whereas, ab is not a palindrome.&nbsp;</p>
<p>Once Gopu was playing with string s, he thought of whether he can change this string into a palindrome or not.</p>
<p>A "cool operation" takes some substring of string with the property that all the characters in the substring should be same. Let us say that substring has size L. Then he can reduce ther size of this substring by alteast 0 and atmost L - 1. eg. string is abbb, He can change substring bbb into b, bb, bbb (corresponding to not changing it at all) which will make the string s into ab, abb, abbb respectively.</p>
<p>He can apply a "cool operation" as many times as he wishes.</p>
<p>Find out whether he can convert the string into a palindrome or not?</p>
<p>Output "YES" if possible, else output "NO".</p>
<h3>Input</h3>
<p>First line of input contains number of test cases T, (1 &lt;= T &lt;= 100).</p>
<p>For each test case, there is a single line representing the string with which Gopu is playing with. (length of string &gt;= 1 and &lt;= 10^5). String will only contain small letters of english alphabet ie 'a' to 'z'.</p>
<h3>Output</h3>
<p>For each test case output a single line containing "YES" or "NO" (without quotes) respectively to situation whether he can convert given string into palindrome or not?</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5<br>aba<br>aabaaa<br>aabbba<br>aaab<br>abca&nbsp;</pre>
<pre><strong>Output:</strong>
YES<br>YES<br>YES<br>NO<br>NO&nbsp;</pre>
<pre><h3>Explanation:</h3><div>For first test case string "aba", string is already a palindrome, so no need to apply "cool operation".</div><div><span style="white-space: pre;">For second test case string "aabaaa", take aaa and convert it into aa, So string becomes aabaa which is a palindrome.</span></div><div><span style="white-space: pre;">For fifth test case string "abca", Gopu can not convert it into palindrome despite applying any "cool operation". </span></div></pre>