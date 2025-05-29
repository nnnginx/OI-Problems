<p> 
The International Olympiad in Informatics is coming and the leaders of the Vietnamese Team have to choose the best contestants all over the country. Fortunately, the leaders could choose the members of the team among N very good contestants, numbered from 1 to N (3 ¡Ü N ¡Ü 100000). In order to select the best contestants the leaders organized three competitions. Each of the N contestants took part in all three competitions and there were no two contestants with equal results on any of the competitions. We say that contestant §¡ is better than another contestant §£ when §¡ is ranked before §£ in all of the competitions. A contestant A is said to be excellent if no other contestant is better than A. The leaders of the Vietnamese Team would like to know the number of excellent contestants.


</p><h3>Input</h3>
<p>
First line of the input contains an integer t (1 ¡Ü t ¡Ü 10 ), equal to the number of testcases. Then descriptions of t testcases follow.
First line of description contains the number of competitors N .
Each of the next N lines describes one competitor and contains integer numbers ai, bi, ci (1 ¡Ü ai, bi , ci ¡Ü N ) separated by spaces, the order of i-th competitor's ranking in the first competition , the second competition and the third competition.
</p><h3>Output</h3>
<p>
For each test case in the input your program should output the number of excellent contestants in one line.
</p>
<p>
<strong>Note:</strong> Because the input is too large so we have 4 input files and the total time limit is 4s ( not 1s ).
</p>
<h3>Example</h3>

<pre><b>Input:</b>
1
3
1 2 3
2 3 1
3 1 2

<b>Output:</b>
3
</pre>