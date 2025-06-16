<p style="font-family: 'Times New Roman'; font-size: medium;">Economic times these days are tough, even in Byteland. To reduce the operating costs, the government of Byteland has decided to optimize the road lighting. Till now every road was illuminated all night long, which costs 1 Bytelandian Dollar per meter and day. To save money, they decided to no longer illuminate every road, but to switch off the road lighting of some streets. To make sure that the inhabitants of Byteland still feel safe, they want to optimize the lighting in such a way, that after darkening some streets at night, there will still be at least one illuminated path from every junction in Byteland to every other junction.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">What is the maximum daily amount of money the government of Byteland can save, without making their inhabitants feel unsafe?</p>
<h4 style="font-family: 'Times New Roman'; font-size: medium;">Input Specification</h4>
<p style="font-family: 'Times New Roman'; font-size: medium;">The input file contains several test cases. Each test case starts with two numbers&nbsp;<strong><em>m</em></strong>&nbsp;and&nbsp;<strong><em>n</em></strong>, the number of junctions in Byteland and the number of roads in Byteland, respectively. Input is terminated by&nbsp;<strong><em>m=n=0</em></strong>. Otherwise,&nbsp;<strong><em>1 ¡Ü m ¡Ü 200000</em></strong>&nbsp;and&nbsp;<strong><em>m-1 ¡Ü n ¡Ü 200000</em></strong>. Then follow&nbsp;<strong><em>n</em></strong>&nbsp;integer triples&nbsp;<strong><em>x, y, z</em></strong>&nbsp;specifying that there will be a bidirectional road between&nbsp;<strong><em>x</em></strong>&nbsp;and&nbsp;<strong><em>y</em></strong>&nbsp;with length&nbsp;<strong><em>z</em></strong>&nbsp;meters (<strong><em>0 ¡Ü x, y &lt; m</em></strong>&nbsp;and&nbsp;<strong><em>x ¡Ù y</em></strong>). The graph specified by each test case is connected. The total length of all roads in each test case is less than 2<sup>31</sup>.</p>
<h4 style="font-family: 'Times New Roman'; font-size: medium;">Output Specification</h4>
<p style="font-family: 'Times New Roman'; font-size: medium;">For each test case print one line containing the maximum daily amount the government can save.</p>
<h4 style="font-family: 'Times New Roman'; font-size: medium;">Sample Input</h4>
<pre>7 11
0 1 7
0 3 5
1 2 8
1 3 9
1 4 7
2 4 5
3 4 15
3 5 6
4 5 8
4 6 9
5 6 11
0 0
</pre>
<h4 style="font-family: 'Times New Roman'; font-size: medium;">Sample Output</h4>
<p><span style="font-family: Verdana, Arial, Helvetica, sans-serif; font-size: 10px;">51</span></p>