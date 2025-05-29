<p>The process of ※<strong>breaking</strong>§ an integer is defined as summing the squares of its digits. For example, the result of breaking the integer <strong>125 </strong>is (<strong>1<sup>2</sup></strong> + <strong>2<sup>2</sup> </strong>+ <strong>5<sup>2</sup></strong>) = <strong>30</strong>. An integer <strong>N</strong> is <strong>happy </strong>if after ※<strong>breaking</strong>§ it repeatedly the result reaches 1. If the result never reaches 1 no matter how many times the ※<strong>breaking</strong>§ is repeated, then N is not a happy number.</p>

<h3>TASK</h3>
<p>Write a program that given an integer <strong>T</strong> (number of test cases) and <strong>T</strong> integers, determines for each number whether it is a happy number or not.</p>

<h3>CONSTRAINTS</h3>
<p><strong>1 ≒ T ≒ 1,080,000</strong></p>
<p><strong>2 ≒ N ≒ 2,147,483,647</strong> (number for determining whether it is happy or not)</p>

<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>.</p>
<p>Next 1...T lines contain an integer <strong>N</strong> for detemining whether it is happy or not.</p>

<h3>Output</h3>
<p>T lines containing a single integer <strong>N</strong> which is the number of times the process had to be done to determine that N is happy, or <strong>-1</strong> if <strong>N</strong> is not happy.</p>

<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>19<br>204<br><br><strong>Output:</strong><br>4<br>-1</pre>

<pre>1) 19  : 1<sup>2</sup> + 9<sup>2</sup> = 82
2) 82  : 82 + 2<sup>2</sup> = 68
3) 68  : 6<sup>2</sup> + 8<sup>2</sup> = 100
4) 100 : 1<sup>2 </sup>+ 0<sup>2</sup> + 0<sup>2</sup> = 1</pre>

<p>The solution for 19 is 4 because we discovered that the integer 19 is happy after we repeated the process 4 times.

</p><pre>204 每&gt; <b>20</b> 每&gt; 4 每&gt; 16 每&gt; 37 每&gt; 58 每&gt; 89 每&gt; 145 每&gt; 42 每&gt; <b>20</b> 每&gt; 4 每&gt; 16 每&gt; 37 每&gt; 58 每&gt; 89 每&gt; 145 ＃＃</pre>
<p><strong>204 </strong>is not a happy number because after breaking it several times the results start repeating so we can deduce that if we continue breaking it, the result will never reach 1.</p>