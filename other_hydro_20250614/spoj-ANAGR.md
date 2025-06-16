<p>Two strings are said to be anagrams of each other if the letters of one string may be rearranged to make the other string.&nbsp; In this problem you¡¯ll be given two strings. Your job is to find if the two strings are anagrams of each other. If they are not anagrams then find the lexicographically smallest palindrome (in lowercase letters) that may be appended to the end of one of the two strings so that they become anagrams of each other.</p>
<p>The lower and upper case letters are considered equivalent. The number of spaces&nbsp; or any other punctuation is not important.</p>
<p><br></p>

<p><strong>INPUT:</strong></p>
<p>The first line of the input contains a number T, the number of test cases. T test cases follow. Each test case consists of two lines, one string in each line.</p>
<p><br></p>

<p><strong>OUTPUT:</strong></p>
<p>For each test case output a single line. Print ¡®YES¡¯ (without the quotes) if the two strings are anagrams of each other. If they are not, then print the lexicographically smallest string as discussed above. If no such string exists, then print ¡®NO LUCK¡¯ (without the quotes).</p>
<p><br></p>

<p><strong>CONSTRAINTS:</strong></p>
<p>1&lt;=T&lt;=100</p>
<p>1&lt;=length of the strings&lt;=100</p>
<p><br></p>

<p><strong>SAMPLE TEST CASES:</strong></p>

<pre><b><u>INPUT:</u></b>

4
Computer programmer
mature germ romp crop
Awaaay
away
internet
web
the terminator
I¡¯m rotten hater

<b><u>OUTPUT:</u></b>

YES
aa
NO LUCK
YES</pre>