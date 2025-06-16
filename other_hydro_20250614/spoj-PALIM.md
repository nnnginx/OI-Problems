<p>A string is called a palindrome if it's the same when read from left to right and from right to left. For example, <tt>"abdba"</tt> is a palindrome, but <tt>"abbaa"</tt> is not.
</p><p>Given a string, print the length of the longest consecutive sequence of characters occurrences at least once in this string, which is a palindrome.

</p><h3>Input</h3>
<ul>
<li>Line 1: a string consists of at most 100000 characters. The ASCII code of all characters are between 32 and 127, inclusive. </li>
<li>Line 2: a magical key(for security purpose).</li>
</ul>

<h3>Output</h3>
<ul>
<li>Line 1: the length of the longest palindrome.</li>
<li>Line 2: the magical key.</li>
</ul>

<h3>Example</h3>

<pre><b>Input:</b>
abaabbabaaba
MAGICAL KEY

<b>Output:</b>
6
MAGICAL KEY
</pre>

<h3>Restriction</h3>
<p>Only C++ is allowed in this problem now. <b>In addition, you will receive <tt>"wrong answer"</tt> if your program don't start with <a href="https://www.spoj.com/content/crazyb0y:PALIM.cpp">this</a>.</b> You can't use macro <tt>"#undef"</tt> in your solution as well.
</p><p>If you want to solve this problem in another language, send me the header file in your language please.
</p><p><b>warning: </b> Don't try to access the memory of tester, or I will reject your solution manually, and you will lose the chance to enjoy this problem as well.
</p><h3>Hint</h3>
<p><b>hint of using tester library: </b>you can't read anything from stdin, and you can't print anything as well, your program will be terminated if you called answer().
</p><p><b>hint of viewing feedback:</b> You can click on <tt>"wrong answer"</tt> link to view the feedback of judge: whether your solution didn't include the testlib, or failed on sample. (if neither, your solution failed on a further test case)
</p><h3>Notice</h3>
<p><b>update on Oct.24: I had updated the header file for C++, now you will receive <tt>"Runtime Error(NZEC)"</tt> if your solution called isSame() illegally. The submissions with old version of header file are still acceptable.</b>
</p><p><b>rejudge on Oct.24:</b> some test cases were added, three submissions were rejudged as TLE instead of AC.
</p>