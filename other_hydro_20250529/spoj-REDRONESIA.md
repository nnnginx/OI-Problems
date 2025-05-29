<p>On the islands of Redronesia, there are many languages spoken.  Each language is made up of a number of words.  And some of the islands are very particular about how the words are formed in their language.</p>
<p>Each language specifies how long a word can be, and how many letters there will be in the alphabet.  But they all insist:</p>
<ul>
<li>that each letter in the word must be at least as big as the previous letter</li>
<li>that doubles of any letter are allowed, but 3 or more of the same letter are not allowed.</li>
</ul>
<p>The aim of the problem is to count the number of possible words.  Since the number may be large, please give the answer mod 1000000007.<br><br>As an example, on the island of Imosua, they have an alphabet of 4 letters (we'll call them a, b, c and d), and 6 letters in each word.  The following words are not allowed on Imosua:</p>
<ul>
<li>aabbc (not 6 letters long)</li>
<li>aabbab (each letter is not at least as big as the previous letter)</li>
<li>aaabbc and aaaabc (triples and longer are not allowed)</li>
</ul>
<p>Some of the 10 allowable words are:</p>
<ul>
<li>aabbcc</li>
<li>aabcdd</li>
<li>bbccdd</li>
</ul>
<h3>Input</h3>
<p>The first line of input contains one integer: T the number of test cases.</p>
<p>On each of the next T lines, your are given two integers: S (the length of each word) and C (the number of characters in the alphabet).</p>
<h3>Output</h3>
<p>For each test case, you have to print the number of possible words.</p>
<p>As the result may be a big number, simply output your result modulo 10^9+7</p>
<h3>Example</h3>
<pre><strong>Input:<br>3<br>6 4<br>6 3<br>6 2</strong>


<strong>Output:<br>10<br>1<br>0<br><br></strong></pre>
<h3><strong>Constraints<br></strong></h3>
<p>1 &lt; T &lt; 100</p>
<p>1 &lt; S, C &lt; 500</p>