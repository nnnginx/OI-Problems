<p align="justify">Alphabet <i>A<sub>k</sub></i> consists of <i>k</i> initial letters of English alphabet. A positive integer called a weight is assigned to each letter of the alphabet. A weight of a word built from the letters of the alphabet <i>A<sub>k</sub></i> is the sum of weights of all letters in this word. A language over an alphabet <i>A<sub>k</sub></i> is any finite set of words built from the letters of this alphabet. A weight of a language is the sum of weights of all its words. We say that the language is prefixless if for each pair of different words <i>w</i>, <i>v</i> from this language <i>w</i> is not a prefix of <i>v</i>. </p>
<p align="justify">We want to find out what is the minimal possible weight of an <i>n</i>-element, prefixless language over an alphabet <i>A<sub>k</sub></i>. </p>

<h3>Example</h3>
<p align="justify">Assume that <i>k</i> = 2, the weight of the letter <tt>a</tt> is <i>W</i>(<tt>a</tt>) = 2 and the weight of the letter <tt>b</tt> is <i>W</i>(<tt>b</tt>) = 5. The weight of the word <tt>ab</tt> is <i>W</i>(<tt>ab</tt>) = 2 + 5 = 7. <i>W</i>(<tt>aba</tt>) = 2 + 5 + 2 = 9. The weight of the language <i>J</i> = {<tt>ab</tt>, <tt>aba</tt>, <tt>b</tt>} is <i>W</i>(<i>J</i>) = 21. The language <i>J</i> is not prefixless, since the word <tt>ab</tt> is a prefix of <tt>aba</tt>. The lightest three-element, prefixless language over the alphabet <i>A</i><sub>2</sub> (assuming that weights of the letters are as before) is {<tt>b</tt>, <tt>aa</tt>, <tt>ab</tt>}; its weight is 16. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads two integers <i>n</i>, <i>k</i> and the weights of <i>k</i> letters of an alphabet <i>A<sub>k</sub></i>; </li>
        <li align="justify">computes the minimal weight of a prefixless, <i>n</i>-element language over the alphabet <i>A<sub>k</sub></i>; </li>
        <li align="justify">outputs the result. </li>
</ul>
</div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there are two positive integers <i>n</i> and <i>k</i> separated by a single space, (2 &lt;= <i>n</i> &lt;= 10000, 2 &lt;= <i>k</i> &lt;= 26). These are the number of words in a language and the number of letters in an alphabet respectively. The second line contains <i>k</i> positive integers separated by single spaces. Each of them is not greater than 10000. The <i>i</i>-th number is the weight of the <i>i</i>-th letter. </p>

<h3>Output</h3>
<p align="justify">For each test case you should output one line with the weight of the lightest prefixless <i>n</i>-element language over the alphabet <i>A<sub>k</sub></i>. </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
3 2
2 5

<b><tt>Sample output:</tt></b>
16
</pre>