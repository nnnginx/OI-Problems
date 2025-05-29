<p>Some people who love strings have decided to call a special group of strings as the <strong>¡°unique strings.¡±</strong></p>
<p>Let¡¯s define <strong>a(S)</strong> as the number of characters ¡°a¡± the string S contains, and <strong>b(S)</strong> as the number of characters ¡°b¡± the string S contains.</p>
<p>S is a unique string if:</p>
<p>1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; S only contains the characters ¡°a¡± and ¡°b¡±</p>
<p>2)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For every substring S¡¯of S, | a(S¡¯) ¨C b(S¡¯) | &lt;= 3</p>
<p>For example, ¡°abbab¡± is a unique string. However, ¡°abbbba¡± is not because it includes the substring ¡°bbbb¡± for which | a(¡°bbbb¡±) ¨C b(¡°bbbbb¡±) | = 4 &gt; 3.</p>
<p>Let¡¯s say we sort the unique strings ¨C <strong>first by length and then lexicographically</strong>. The N<sup>th</sup> unique string is the string that appears in the position N in the sorted list. The first unique string is assigned the number 1.</p>
<p>The first 12 unique strings in the sorted list are: <strong>a, b, aa, ab,ba, bb, aaa, aab,&nbsp; aba, abb, baa, bab</strong></p>
<h3>Input</h3>
<p>A single number N (1 &lt;= N &lt;= 10<sup>14</sup>). Your task is to find the N<sup>th</sup> unique string in the sorted list.</p>
<h3>Output</h3>
<p>A single line: the N<sup>th</sup> unique string in the sorted list.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10

<strong>Output:</strong>
abb</pre>
<pre>_______</pre>
<pre><strong>Input:</strong></pre>
<pre>19</pre>
<pre><strong>Output:</strong></pre>
<pre>abab</pre>