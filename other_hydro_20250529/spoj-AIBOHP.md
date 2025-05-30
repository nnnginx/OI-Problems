<p>BuggyD suffers from AIBOHPHOBIA - the fear of Palindromes.  A palindrome is a string that reads the same forward and backward.</p>

<p>To cure him of this fatal disease, doctors from all over the world discussed his fear and decided to expose him to large number of palindromes.  To do this, they decided to play a game with BuggyD.  The rules of the game are as follows:</p>

<p>BuggyD has to supply a string <b>S</b>. The doctors have to add or insert characters to the string to make it a palindrome.  Characters can be inserted anywhere in the string.</p>

<p>The doctors took this game very lightly and just appended the reverse of <b>S</b> to the end of <b>S</b>, thus making it a palindrome.  For example, if <b>S</b> = <tt>"fft"</tt>, the doctors change the string 
to <tt>"ffttff"</tt>.</p>

<p>Nowadays, BuggyD is cured of the disease (having been exposed to a large number of palindromes), but he still wants to continue the game by his rules. He now asks the doctors to insert the minimum number of characters needed to make <b>S</b> a palindrome.  Help the doctors accomplish this task.</p>

<p>For instance, if <b>S</b> = <tt>"fft"</tt>, the doctors should change the string to <tt>"tfft"</tt>, adding only 1 character.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>Each test case consists of one line, the string <b>S</b>.  The length of <b>S</b> will be no more than 6100 characters, and <b>S</b> will contain no whitespace characters.</p>

<h3>Output</h3>

<p>For each test case output one line containing a single integer denoting the minimum number of characters that must be inserted into <b>S</b> to make it a palindrome.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
fft

<b>Output:</b>
1
</pre>