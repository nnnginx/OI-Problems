<p style="text-align: justify;">Hugo had quite a bad day today. His favourite highschool subject, mathematics, was taught by his least liked substitute teacher - he always gave out an abnormally large amount of homework. Today was no different.</p>
<p style="text-align: justify;">The teacher wrote <strong>N</strong> numbers on the board, and after a long thoughtful pause he told the class with a grin: "Well then, kids. For today's homework you will do this harmless exercise. As you can see, I've written quite a few numbers on the board, and your task is to find which two of them have the greatest product. Hm,  now that I think about it, that would be too trivial. So you will also have to find which pair of numbers has  the greatest quotient. Well, and now that we're at it, why don't you find the pair with the smallest quotient, too. And at that point you might as well find the pair with the smallest product. That should keep you busy  for today's evening!". <br><br>Sigh.<br> How could someone even come up with such a boring, time-consuming and impractical task. If only there was someone who would help Hugo and do it for him.</p>
<h3>Input</h3>
<p style="text-align: justify;">The first line of input contains the number <strong>1 ¡Ü T ¡Ü 15</strong>: the number of test cases. <strong>T</strong> cases follow.<br>The first line of each case contains the number <strong>2 ¡Ü N ¡Ü 10<sup>5</sup></strong>: how many numbers the teacher wrote on the board. The second line contains <strong>N</strong> integers; their absolute value will be in the range <strong>[1,10<sup>6</sup>]</strong> (inclusive). In particular, notice that none of them are equal to zero.<br>You may assume that in any input file, the sum of <strong>N</strong> across all test cases does not exceed <strong>3*10<sup>5</sup></strong>.</p>
<h3><strong>Output</strong></h3>
<p style="text-align: justify;">For each case, output five lines. The first one contains the number of the case x in the format "Case x:", starting at 1.</p>
<p style="text-align: justify;">Then output four lines, each containing two integers from the input (let's call them <strong>x</strong> and <strong>y</strong>). They need to have the following properties (in this order):</p>
<p style="text-align: justify;"><strong>x * y</strong> is the greatest possible<br> <strong>x * y</strong> is the lowest possible<br> <strong>x / y</strong> is the greatest possible<br> <strong>x / y</strong> is the lowest possible</p>
<p style="text-align: justify;">If there are multiple pairs of integers which fulfill the criteria, output the one with the lowest <strong>x</strong>.<br> <strong>x,y</strong> may be equal, but in that case their value has to appear at least twice in the input.<br> All four lines are independent, that is the same integer from the input may be used across multiple lines.<br> A number <em>A</em> is said to be greater than <em>B</em> if <em> A &gt; B </em> and lower than <em>B</em> if <em> A &lt; B</em>.</p>
<h3><strong>Example</strong></h3>
<pre><strong>Input:</strong>
1
3
5 -7 10
<strong>Output:</strong>
Case 1:
5 10
-7 10
10 5
10 -7
</pre>