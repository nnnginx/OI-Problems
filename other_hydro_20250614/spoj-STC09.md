<p>Let us consider a text consisting of N&nbsp;words numbered from 1&nbsp;to N. We represent any of its decompositions into&nbsp;<span>K</span>&nbsp;lines by a sequence of numbers&nbsp;<span>(a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ..., a<sub>k-1</sub>)</span>, such that the words with numbers from 1&nbsp;to a<sub>1</sub>&nbsp;are in the first line, the words with numbers from a<sub>1</sub>+1&nbsp;to a<sub>2</sub>&nbsp;are in the second line, and so on, and finally, the words with numbers from a<sub>K</sub>-1&nbsp;to N&nbsp;are in the last, K-th line.</p>
<p>Each word has a certain length (measured in the number of characters). Let length(x)&nbsp;denote the length of the word no. x. Furthermore, every two subsequent words in a line are separated by a space of width of a single character. By length of the line we denote the sum of lengths of the words in this line, increased by the number of spaces between them. Let line(w)&nbsp;denote the length of the line no. w. I.e., if the line no. w&nbsp;contains the words with numbers from i&nbsp;to j&nbsp;inclusive, its length is:</p>
<p style="text-align: center;">line(w)=length(i)+length(i+1)+...+length(j)+(j-i)</p>
<p>As an example, let us consider a text consisting of 4&nbsp;words of lengths 4, 3, 2&nbsp;and 5, respectively, and its decomposition (1, 3)&nbsp;into 3&nbsp;lines. Then the length of the first line is 4, second - 6, and third - 5:</p>
<p style="text-align: center;"><tt>XXXX&nbsp;</tt>(1st line)<br><tt>XXX XX&nbsp;</tt>(2nd line)<br><tt>XXXXX&nbsp;</tt>(3rd line)</p>
<p>We shall refer to the number</p>
<p style="text-align: center;">|line(1)-line(2)|+|line(2)-line(3)|+...+|line(K-1)-line(K)|</p>
<p>as the coefficient of aestheticism of a decomposition of the given text into K&nbsp;lines. Particularly, if the decomposition has only one line, its coefficient of aestheticism is 0.</p>
<p>Needles to say, the smaller the coefficient, the more aesthetical the decomposition. We shall consider only these decompositions that have no line whose length exceeds some constant M. Of all such decompositions of a given text into any number of lines we seek the one most aesthetical, i.e. the one with the smallest coefficient of aestheticism. The aforementioned examplary decomposition's coefficient is 3, and that is exactly the minimum coefficient of aestheticism for M = 6&nbsp;and M = 7.</p>
<p>&nbsp;</p>
<h2>Task</h2>
<p>Write a programme that:</p>
<ul>
<li>reads from the standard input the numbers N&nbsp;and M&nbsp;and the lengths of the words,</li>
<li>determines the minimum coefficient of aestheticism for those decompositions, whose every line is of length not exceeding M,</li>
<li>writes the result to the standard output.</li>
</ul>
<p>&nbsp;</p>
<h2>Input</h2>
<p>The first line of the standard input contains the numbers N&nbsp;and M, 1 &lt;= N &lt;= 2000, 1 &lt;= M &lt;= 1000000, separated by a single space. The second, last line of the standard input contains M&nbsp;integers, denoting the lengths of subsequent words, 1 &lt;= length(i) &lt;= M&nbsp;for i = 1, 2, 3, ... M, separated by single spaces.</p>
<h2>Output</h2>
<p>The first and only line of the standard output should contain exactly one integer: the minimum coefficient of aestheticism for those decompositions, whose every line's length does not exceed M.</p>
<p>&nbsp;</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>6 4
4 3 2 5</pre>
<p>the correct result is:</p>
<pre>3</pre>
<p>while for the following input data:</p>
<pre>4 2
1 2</pre>
<p>the correct result is:</p>
<pre>0</pre>