<p>A word ring is a sequence of words where the last two letters of each word are the same as the first two letters of the next word (and the last two letters of the last word are the same as the first two letters of the first word). For example, the following sequence is a word ring: </p>
<pre>intercommunicational
alkylbenzenesulfonate
tetraiodophenolphthalein
</pre>
<p>Your task is to write a program that, given a list of words, finds a word ring. You have to make the word ring as impressive as possible: the average length of the words in the ring has to be as large as possible. In the above example, the average length is (20 + 21 + 24)/3 = 21.6666 , which makes it somewhat impressive. Note that each word can be used at most once in the ring, and the ring can consist of a single word.</p>

<h3>Input</h3>

<p>The input contains several blocks of test cases. Each case begins with a line containing a single integer 1 &lt;= n &lt;= 100000 , the number of possible words that can be used. The next n lines contain these words. The words contain only the characters 'a'-'z' and the length of each word is at most 1000.

</p><p>The input is terminated by a block with n = 0.</p>

<h3>Output</h3>

<p>For each test case in the input, you have to output a single number on a separate line: the maximum average length of a ring composed from (a subset of) the words given in the input. The average length should be presented as a real number with two digits of precision. If it is not possible to compose a ring from these words, then output 'No solution.' (without quotes). To avoid rounding problems, we accept solutions with a maximum of 0.01(positive or negative) error. </p>
<h3>Example</h3>
<pre><b>Input:</b>
3
intercommunicational
alkylbenzenesulfonate
tetraiodophenolphthalein
0

<b>Output:</b>
21.66
</pre>
<b>Warning: large input/output data, be careful with certain languages</b>