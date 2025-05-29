<p>Fernando is president of country named Palindromia. Every two years there are elections in Palindromia, but not normal elections. Elections in Palindromia are preformed in next steps:</p>
<ul>
<li>Candidate which at the moment isn't president gives to the current president one string <strong><em>O,</em></strong> which consist only of upper-case letters of english alphabet and character '?', string <em><strong>U,</strong></em> which consist only of upper-case letters of english alphabet, and integer <strong><em>K</em></strong>. </li>
</ul>
<ul>
<li>Current president has one day to compute all longest palindromes in the first string by the folowing rules:        <br> 
<ul>
<li>Every '?' in <em><strong>O</strong></em> is substituted with one letter from <em><strong>U</strong></em>, <em><strong>i</strong></em>-th '?' in <strong><em>O</em></strong> with <strong><em>i</em></strong>-th letter in <em><strong>U</strong></em>.</li>
<li>Every time he search for palindromes, he may substitute some '?' with any letter, at most <em><strong>K</strong></em>-times.</li>
<li>If he finds palindrome, he goes to step 1.</li>
</ul>
</li>
</ul>
<ul>
<li>If he doesn't succeed, the candidate becomes the new president </li>
</ul>
<ul>
<li>If there are more candidates, go to step one.</li>
</ul>
<p>Fernando wants to stay president for at least two more years, so he asks you to write program which solves his problem.</p>
<blockquote><ol> </ol> 
<ul>
</ul>
<blockquote><ol> </ol></blockquote>
<ul>
</ul>
</blockquote>
<blockquote><br>
<h3>Input</h3>
<p>First line of input will contain string <em><strong>O</strong></em> ( 1 &lt;= lenght of <strong><em>O</em></strong> &lt;= 5 * 10^5 ), string which Fernando must compute to stay president. <em><strong>O</strong></em> will consist only of upper-case letters of english alphabet and character '?'. You may assume there is at least one '?' in <em><strong>O</strong></em>.</p>
<p>Second line will contain string <em><strong>U</strong></em>, string with leads for '?'s. <em><strong>i</strong></em>-th letter in <em><strong>U</strong></em> corespond to <em><strong>i</strong></em>-th '?' in <strong><em>O</em></strong>. <em><strong>U</strong></em> will consist only of upper-case letters of english alphabet.</p>
<p>Third line will contain integer <em><strong>K</strong></em> ( 0 &lt;= K &lt;= 300 ), number of replacements.</p>
<p><span style="font-size: large;"><strong><em><span style="text-decoration: underline;">It is guraranteed that there will be not more than 300 '?'s.</span></em></strong></span></p>
<h3>Output</h3>
<p>In first line of output print integer <em><strong>S</strong></em>, lenght of the longest palindrome that Fernando could find.</p>
<p>In Second and next lines print string <em><strong>P</strong><strong><sub>i</sub></strong></em> and integer <strong><em>L<sub>i</sub>, </em></strong>longest palindrome and position where it starts. Each <em><strong>P</strong><strong><sub>i</sub></strong></em> must contain only upper-case letters of english alphabet.</p>
<p>&nbsp;</p>
<p><strong>Notes:</strong></p>
<ul>
<li>you must print all longest palindromes, in alphabeticaly increasing order</li>
<li>if two or more palindromes starts at the same position, print only one of them</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong><br>UDOVICAB??IVODUANAVOL?MILOVANA<br>CCA<br>1<br><br><strong>Output:</strong><br>15<br>ANAVOLIMILOVANA 16<br>UDOVICABACIVODU 1<br><br><span style="text-decoration: underline;"><span style="font-size: small;"><em><strong><br><span style="font-size: large;">Note that both palindromes have 1 letter which Fernando has changed.</span></strong></em></span><br></span><br><br><br><strong>Input:<br></strong>ABCDE??ABCDE??<br>ABCD<br>1<br><strong><br>Output:</strong><br>5<br>CBABC 6<br><br><br><strong>Input:</strong><br>ABCDE??ABCDEFG<br>FG<br>0<br><br><strong>Output:</strong><br>1<br>A 1<br>A 8<br>B 2<br>B 9<br>C 10<br>C 3<br>D 4<br>D 11<br>E 5<br>E 12<br>F 13<br>F 6<br>G 7<br>G 14<br><br></pre>
</blockquote>