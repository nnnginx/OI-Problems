<p><span style="font-size: small;">The King of DragonStone is known for his dragons and magic. It can be very hardand dangerous to tame a dragon. So, in order to control his dragons The King speaks random but powerful words. The strength of his words is determined by a strange rule. Rule : Strength of a word is sum of cube of length of palindromic substrings in the word. To recall the definition of palindrome, palindrome is a word which reads same when read forward and backward. For example, word "abaa" has 6 palindromic substrings. "aba","aa","a","b","a","a" with sizes 3,2,1,1,1,1 respectively. Their cubes are 27,8,1,1,1,1. Hence total strength is 39. Given a King's word, find its strength.</span></p>
<h3>Input</h3>
<p><span style="color: #252c33; word-spacing: 1px;"><span style="font-size: small;">First line of input contains an integer T, the number of test cases. Followed by T lines, each line containing a word(say S).(only lowercase letters are allowed).</span></span></p>
<p style="color: #252c33; font-family: &quot;Open Sans&quot;, sans-serif; font-size: 14px; word-spacing: 1px;"><span style="font-weight: 600;"><span style="font-size: x-small;">Constraints:</span></span></p>
<p style="color: #252c33; word-spacing: 1px;"><span style="font-size: small;">1 &lt;= length of word &lt;= 1000</span></p>
<p style="color: #252c33; word-spacing: 1px;"><span style="font-size: small;">1 &lt;=&nbsp;T &lt;= 100</span></p>
<h3>Output</h3>
<p><span style="color: #252c33; font-family: &quot;Open Sans&quot;, sans-serif; font-size: 14px; word-spacing: 1px;">For every word (S), output a single line containing the strength of the word.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2 </pre>
<pre>abaa </pre>
<pre>dbd </pre>
<pre><p style="color: #252c33; font-family: &quot;Open Sans&quot;, sans-serif; font-size: 14px; word-spacing: 0px;"><span style="font-weight: bold; color: #000000; font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px;">Output:</span></p><p style="color: #252c33; font-size: 14px; word-spacing: 0px; text-align: justify;"><span style="font-family: verdana, geneva;"><span style="font-size: xx-small;">39 </span></span></p><p style="color: #252c33; font-size: 14px; word-spacing: 1px; text-align: justify;"><span style="font-family: verdana, geneva;"><span style="font-size: xx-small;">30</span></span></p><p style="color: #252c33; font-size: 14px; word-spacing: 1px; text-align: justify;"><strong><br></strong></p><p style="color: #252c33; font-size: 14px; word-spacing: 1px; text-align: justify;"><strong>Note: There is no space between lines</strong></p>
</pre>