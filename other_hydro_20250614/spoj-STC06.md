<p>Byteman has received an extraordinary keyboard as a gift. The keyboard is a rectangle consisting of N&nbsp;rows and M&nbsp;columns with N*M&nbsp;keys placed on it. Moreover, all keys except the one in the top left corner are covered with domino tiles of size 1 x 2, so there are (N*M-1)/2&nbsp;domino tiles in total. At any time, Byteman can move onto the free key one of the domino tiles adjacent to it by the shorter side. He can also press keys, but only if they are not covered.</p>
<p>Byteman would like to test (i.e., press) all the keys corresponding to vowels, that is, the letters&nbsp;<tt>a</tt>,&nbsp;<tt>e</tt>,&nbsp;<tt>i</tt>,&nbsp;<tt>o</tt>,&nbsp;<tt>u</tt>&nbsp;or&nbsp;<tt>y</tt>. What is the minimum number of tile moves necessary to do that?</p>
<h2>Input</h2>
<p>The first line of the input contains two integers N&nbsp;and M&nbsp;(1 &lt;= N,M &lt; 70) that describe the dimensions of the keyboard. The next N&nbsp;lines contain M&nbsp;lowercase letters of the English alphabet each, describing the rows of the keyboard. Each of the next N&nbsp;lines contains M&nbsp;characters describing placement of the domino tiles:&nbsp;<tt>.</tt>&nbsp;(ASCII code 46) denotes an uncovered key,&nbsp;<tt>-</tt>&nbsp;(ASCII code 45) denotes a key covered by a domino tile placed horizontally and&nbsp;<tt>|</tt>&nbsp;(ASCII code 124) - a key covered by a tile placed vertically.</p>
<h2>Output</h2>
<p>If it is not possible for Byteman to press all the keys corresponding to vowels, your program should output just the single word "<tt>NIE</tt>" (i.e.&nbsp;<em>no</em>&nbsp;in Polish). Otherwise output the minimum number of tile moves that Byteman must make in order to press all the requested keys.</p>
<h2>Example</h2>
<p>For the input data:</p>
<pre>3 3
ytr
hgf
dsa
.--
|||
|||</pre>
<p>the correct result is:</p>
<pre>2</pre>