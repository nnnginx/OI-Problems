<p>Irena and Sirup are organizing their engagement party next weekend. They want to invite almost everybody. They have just bought a very big round table for this occasion. But they are now wondering how should they distribute people around the table. Irena claimed that when there are more than K women next to each other, this group will chat together for the whole night and won't talk to anybody else.
</p><p>Sirup had no other choice but to agree with her. However, being a mathematician, he quickly became fascinated by all the possible patterns of men and women around the table.</p>
<h3>Problem specification</h3>
<p>There will be N people sitting at the round table. Some of them will be men and the rest will be women. 
</p><p>Your task is to count in how many ways it is possible to assign the places to men and women in such a way that there will not be more than K women sitting next to each other. 
</p><p>If one assignment can be made from another one by rotating all the people around the table, we consider them equal (and thus count this assignment only once).</p>
<h3>Input specification</h3>
<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line. 
</p><p>The input for each test case consists of a single line that contains the two integers N(1&lt;= N &lt;1000) and K.</p>
<h3>Output specification</h3>
<p>For each test case output a single line with one integer ¨C the number of ways how to distribute people around the table, modulo 100000007.</p>
<h3>Example</h3>
<pre><b>input:</b>
3

3 1

3 3

4 1

<b>output:</b>
2
4
3
</pre>
<b>Hint:</b>
<p>In the first test case there are two possibilities: MMM or MMW (M is a man, W is a woman). 
</p><p>In the second test case there are two more possibilities: MWW and WWW. 
</p><p>In the third test case the three possibilities are: MMMM, MMMW, and MWMW.</p>
<p><b>A Note:</b> There are almost 1000 test cases, most of which are randomly generated (huge) ones.</p>