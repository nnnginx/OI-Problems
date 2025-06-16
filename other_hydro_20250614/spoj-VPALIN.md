<p>A word is called a palindrome if we read from right to left is as same as we read from left to right. For example, "dad", "eye" and "racecar" are all palindromes, but "odd", "see" and "orange" are not palindromes. </p>

<p>Given n palindromes, you can generate n ¡Á n pairs of them and concatenate the pairs into single words. The task is to count how many of the so generated words are palindromes.</p>

<h3>Input</h3>
<p>The first line of input file contains the number of strings n. The following n lines describe each string:

The i+1-th line contains the length of the i-th string li, then a single space and a string of li small letters of English alphabet.

You can assume that the total length of all strings will not exceed 2,000,000. Two strings in different line may be the same. </p>

<h3>Output</h3>
<p>Print out only one integer, the number of palindromes. </p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 a
2 bb
2 aa


<b>Output:</b>
5
The 5 palindromes are:
aa aaa aaa bbb aaaa 
</pre>