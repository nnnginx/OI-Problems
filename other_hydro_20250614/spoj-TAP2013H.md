<p><strong><em>[The original version of this problem (in Spanish) can be found at <a title="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf" href="http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/tap2013-problems.pdf</a>]</em></strong></p>
<p>Horace likes to play writing natural numbers in the blackboard in his bedroom. One of his favourite games consists in first writing a number <strong>n</strong>, then the sum of all the different prime numbers that divide <strong>n</strong>, and so on until the number written on the board becomes a prime number. For example, if Horace begins writing the number <strong>n = 90</strong>, because <strong>90 = 2&nbsp;��&nbsp;3<sup>2</sup>&nbsp;��&nbsp;5</strong> the next number to be written will be <strong>2 + 3 + 5 = 10</strong>; then,&nbsp;as&nbsp;<strong>10 = 2 ��&nbsp;5</strong> Horace will write the number <strong>2 + 5 = 7</strong>; finally, because <strong>7</strong> is a prime number the game will end here.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Formally, in this game each natural number n &gt;= 2 defines a sequence whose first element is n, and each new element is the sum of all the prime numbers that divide the previous element in the sequence. The order of the game is the position of the first prime number in the sequence, and coincides with the total number of numbers written on the blackboard one the game has ended. In the example from the previous paragraph, with n = 90 the order of the game is K = 3, because the numbers that are written will be 90, 10 and 7.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now, not all games are equally entertaining to Horace, and in this case he prefers to begin by writing a number n such that the order of the corresponding game is a particular value K. Horace would like to know how many different values of n between A and B inclusive satisfy this condition, but because he does not know how to code he needs someone to do this calculation for him. Can you help him?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains an integer P which indicates the number of questions Horace wants to ask you (1 &lt;= P &lt;= 10^5). Each of the next P lines describes a question using three integer numbers A, B and K, which mean that Horace would like to know how many different values of n satisfy that A &lt;= n &lt;= B and the order of the game beggining with n is K (2 &lt;= A &lt;= B &lt;= 10^6 and 1 &lt;= K &lt;= 10^6).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You should print P lines, each one containing an integer number with the answer to one of the questions made by Horace, in the order in which they appear in the input.</div>
<p>Formally, in this game each natural number <strong>n ��&nbsp;2</strong> defines a sequence whose first element is <strong>n</strong>, and each new element is the sum of all the prime numbers that divide the previous element in the sequence. The order of the game is the position of the first prime number in the sequence, and coincides with the total amount of numbers written on the blackboard once the game has ended. In the example from the previous paragraph, with <strong>n = 90</strong> the order of the game is <strong>K = 3</strong>, because the numbers that are written will be <strong>90</strong>, <strong>10</strong> and <strong>7</strong>.</p>
<p>Now, not all games are equally entertaining to Horace, and in this case he prefers to begin by writing a number <strong>n</strong> such that the order of the corresponding game is a particular value <strong>K</strong>. Horace would like to know how many different values of <strong>n</strong> between <strong>A</strong> and <strong>B</strong> inclusive satisfy this condition, but because he does not know how to code he needs someone to do this calculation for him. Can you help him?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>P</strong> which indicates the number of questions Horace wants to ask you (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;P ��&nbsp;10<sup>5</sup></strong>). Each of the next <strong>P</strong> lines describes a question using three integer numbers <strong>A</strong>, <strong>B</strong> and <strong>K</strong>, which mean that Horace would like to know how many different values of <strong>n</strong> satisfy that <strong>A&nbsp;</strong><strong>��</strong><strong>&nbsp;n&nbsp;</strong><strong>��</strong><strong>&nbsp;B</strong> and the order of the game beginning with <strong>n</strong> is <strong>K</strong> (<strong>2&nbsp;</strong><strong>��</strong><strong>&nbsp;A&nbsp;</strong><strong>��</strong><strong>&nbsp;B&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>6</sup></strong> and <strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;K&nbsp;</strong><strong>��&nbsp;</strong><strong>10<sup>6</sup></strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>You should print <strong>P</strong> lines, each one containing an integer number with the answer to one of the questions made by Horace, in the order in which they appear in the input.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">1
90 90 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1</span></pre>
<pre><span style="font-family: 'courier new', courier;"><br></span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5
2 9 1
2 9 2
800 810 4
999999 1000000 2
100000 1000000 1000000</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">4
4
5
2
0</span></pre>