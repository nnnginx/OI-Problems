<p>Little Daniel loves to play with strings! He always finds different ways to have fun with strings! Knowing that, his friend Kinan decided to test his skills so he gave him a string <strong>S</strong> and asked him <strong>Q</strong> questions of the form:</p>
<p><br>If all distinct substrings of string <strong>S</strong> were sorted lexicographically, which one will be the <strong>K-th</strong> smallest?</p>
<p><br>After knowing the huge number of questions Kinan will ask, Daniel figured out that he can't do this alone. Daniel, of course, knows your exceptional programming skills, so he asked you to write him a program which given <strong>S</strong> will answer Kinan's questions.<br><strong><br>Example:</strong></p>
<p><br><strong>S</strong> = "aaa" (without quotes)<br>substrings of S are "a" , "a" , "a" , "aa" , "aa" , "aaa". The sorted list of substrings will be:<br>"a", "aa", "aaa".</p>
<p>&nbsp;</p>
<h3 style="text-align: center;">Input</h3>
<p>In the first line there is Kinan's string <strong>S</strong> (with length no more than  90000 characters). It contains only small letters of English alphabet.  The second line contains a single integer <strong>Q</strong> (<strong>Q</strong> &lt;= 500) , the number of questions Daniel will be asked. In the next <strong>Q</strong> lines a single integer <strong>K</strong> is given (0 &lt; <strong>K</strong> &lt; 2^31).</p>
<h3 style="text-align: center;">Output</h3>
<p>Output consists of <strong>Q</strong> lines, the <strong>i-th </strong>contains a string which is the answer to the <strong>i-th</strong> asked question.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>aaa<br>2<br>2<br>3<br><br><strong>Output:</strong>
aa<br>aaa<br></pre>

<p><b>Edited:</b> Some input file contains garbage at the end. Do not process them. </p>