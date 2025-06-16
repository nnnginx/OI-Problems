<p>Byteasar breeds hamsters. Each hamster has a unique name, consisting of lower case letters of the English alphabet. The hamsters have a vast and comfortable cage. Byteasar intends to place a display under the cage to visualize the names of his hamsters. This display is simply a sequence of letters, each of which can be either lit or not independently. Only one name will be displayed simultaneously. The lit letters forming the name have to stand next to each other, i.e., form a contiguous subsequence.</p>
<p>Byteasar wants to be able to display the names of the hamsters on at least M&nbsp;different positions. However, he allows displaying the same name on multiple different positions, and does not require to be able to display each and every hamster's name. Note that the occurrences of the names on the display can overlap. You can assume that no hamster's name occurs (as a contiguous fragment) in any other hamster's name. Bytesar asks your help in determining the minimum number of letters the display has to have.</p>
<p>In other words, you are to determine the minimum length of a string (consisting of non-capital letters of the English alphabet) that has at least M&nbsp;total occurrences of the hamsters' names (counting multiplicities). (We say that a string S&nbsp;occurs in the string T&nbsp;if S&nbsp;forms a contiguous fragment of T.)</p>
<h2>Input</h2>
<p>The first line of the standard input holds two integers N&nbsp;and M&nbsp;(1&lt;=N&lt;=200, 1&lt;=M&lt;=10<sup>9</sup>), separated by a single space, that denote the number of Byteasar's hamsters and the minimum number of occurrences of the hamsters' names on the display. Each of the following N&nbsp;lines contains a non-empty string of non-capital letters of the English alphabet that is the hamster's name. The total length of all names does not exceed 10<sup>5</sup>&nbsp;letters.</p>
<h2>Output</h2>
<p>The first and only line of the standard output should hold a single integer - the minimum number of letters the display has to have.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>4 5
monika
tomek
szymon
bernard</pre>
<p>the correct result is:</p>
<pre>23</pre>
<p>The shortest display could be, for example:&nbsp;<tt>szymonikatomekszymonika</tt>. It has 5 occurrences of the hamsters' names in total:&nbsp;<tt>szymon</tt>&nbsp;and&nbsp;<tt>monika</tt>&nbsp;occur twice each,&nbsp;<tt>tomek</tt> just once, and&nbsp;<tt>bernard</tt>&nbsp;does not occur in it at all.</p>