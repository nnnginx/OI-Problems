<p>Harry Potter was punished for his impudence by Snape and was sent to the forbidden forest for detention. He has now lost his way amidst the forest. He has come across 3 mystical rivers flowing in his way to the school but he is not sure which river does he have to cross.
Alongside each mystical river are stones after every meter with a number written on them. The numbers start with 1, 3 and 9 respectively for the three rivers. The number on a stone is equal to the no. on the previous stone plus the sum of its digits. For example, if one no. is 403 then the next no. is 403+4+0+3=410, the next no. is 410+4+1+0=415 and so on. Harry calls this a ��stone river��.
Harry knows that he has to cross at the stone number which is part of the stone river of the number he remembers. He has to now find the point of intersection of the stone river generated by the no. ��N�� that he remembers, with the rivers of 1 or 3 or 9.
Your task is to find which mystical river intersects the stone river generated by Harry��s number. Also find the point of intersection at which Harry can cross the mystical river.
For example, if Harry remembers that he has to cross at the stone number which is part of the stone river of 29 then he has to cross at the stone number 107 which is also in the river of number 1.
Stone river of 29: 29,40,44,52,59,73,83,94,107,��.
River of 1: 1,2,4,8,16,23,28,38,49,62,70,77,91,101,103,107,��.
Both the rivers meet at 107 and hence Harry has to cross at stone number 107.

It is possible that the stone river might intersect with more than one of the mystical rivers. In that case, output the least intersection number.

</p><h3>Input</h3>
<p>The first line consists of a single integer ��T�� (1&lt;=T&lt;=50) which is the total number of test cases. Each of the next T lines consist of a single integer ��N�� (1&lt;=N&lt;=99999999) which is the number that Harry remembers.

</p><h3>Output</h3>
<p>A total of T lines, where each line consists of two integers separated by a space. The first integer represents the river out of 1, 3 and 9 which intersects with the stone river of ��N��. The second integer represents the stone number at which Harry can cross.
</p><h3>Example</h3>

<pre><b>Input:</b>
2
29
42

<b>Output:</b>
1 107
3 111
</pre>