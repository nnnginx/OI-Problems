<p style="text-align: justify;">Hugo had quite a bad day today. His favourite university subject, mathematical analysis, was taught by his least liked substitute teacher - he always gave out an abnormaly large amount of homework. Today was no different.</p>
<p style="text-align: justify;">The teacher wrote <strong>N</strong> numbers on the board, and after a long, thoughtful pause he told the class with a grin: "Well then, kids. For today's homework you will do this harmless exercise. As you can see, I've written quite a few numbers on the board, and your task is to find which smallest non-empty subset of them has the greatest product. That should keep you busy  for today's evening!". <br><br>Sigh.<br> How could someone even come up with such a boring, time-consuming and impractical task. If only there was someone who would help Hugo and do it for him.</p>
<h3>Input</h3>
<p style="text-align: justify;">The first line of input contains the number <strong>1 ¡Ü T ¡Ü 15</strong>: the number of test cases. <strong>T</strong> cases follow.<br>The first line of each case contains the number <strong>1 ¡Ü N ¡Ü 10<sup>5</sup></strong>: how many numbers the teacher wrote on the board. The second line contains <strong>N</strong> integers; their absolute value will not exceed <strong>10<sup>9</sup></strong>.<br>You may assume that in any input file, the sum of <strong>N</strong> across all test cases does not exceed <strong>3*10<sup>5</sup></strong>.</p>
<h3><strong>Output</strong></h3>
<p>For each test case, first print the string 'Case x: ', where x is the number of the test case, starting with 1. Then print a binary string (consistring of <strong>0</strong>'s and <strong>1</strong>'s) ; the <strong>i<sup>th</sup></strong> character should be <strong>1</strong> if you decided to include the  <strong>i<sup>th</sup></strong> number from the input in the subset.</p>
<p>To make the output unambiguous, it should have the following properties:</p>
<ol>
<li>It should contain <strong>N</strong> characters, at least one of which has to be a <strong>1</strong>.</li>
<li> If we multiply the numbers from the input at whose indices this string has the character <strong>1</strong>, the result will be the greatest possible. </li>
<li> Out of all binary strings with the above properties, it should contain the minimum number of <strong>1</strong>'s.</li>
<li> Out of all binary strings with the above properties, it should be lexicographically largest. </li>
</ol>
<p>Reminder: To compare two valid strings lexicographically, find the first position from the left at which they differ. The one with a <strong>1</strong> at this position is lexicographically larger.</p>
<p>&nbsp;</p>
<h3><strong>Example</strong></h3>
<pre><strong>Input:</strong>
1
6
-2 -2 -3 4 5 1
<strong>Output:</strong>
Case 1: 101110
</pre>
<p>The product of the subset this string represents is <strong>(-2) * (-3) * 4 * 5 = 120</strong>, which is the greatest possible. It uses the first -2 from the input, as using the second one would result in a lexicographically smaller string. It does not use the 1, as the product would remain the same but the number of <strong>1</strong>'s in the string would increase.</p>