<p>Filch¡¯s Dilemma (15 points)

Argus Filch, the caretaker of Hogwarts, has been given the task to carpet the way to Hogwarts through the grounds. The way is 2 units wide and ¡®N¡¯ units long. He has only two types of carpets available, one is 1 unit wide and 2 units long and the other one is L shaped, having 3 square units. Here are their pictures:
<br>
<img src="./21702/file/LtmzYhjg.png" style="display:block; margin-left:auto; margin-right:auto;">
<br>
Filch can rotate the carpets when he lays them and has an infinite supply of both types of carpets.
As Filch is a squib he cannot magically arrange the carpets and has to resort to logic to find out all possible ways of carpeting the way. He wishes to calculate the number of different ways of carpeting the way.<br>
For instance, a 2x3 way can be carpeted in 5 different ways as follows:<br>
<br>
<img src="./21702/file/xMiJdKsY.png" style="display:block; margin-left:auto; margin-right:auto;">
<br>
Notice that both types of carpets can be used simultaneously. Consider, for instance the following way of carpeting a 2x4 way:<br>
<br>
<img src="./21702/file/g0xbIJPy.png" style="display:block; margin-left:auto; margin-right:auto;">
<br>
Given N, you have to help Filch determine the number of ways to carpet the way of size 2xN. Since this number may be very large, it is sufficient to report the last four digits of the answer. For instance the number of ways to carpet a 2x13 way is 13465. Your program should just print 3465. If the answer is in 4 digits or less it should print the entire answer. For example, if N=3 you should print 5.<br>


</p><h3>Input</h3>
<p>The first line of the input consists of a single integer T(1&lt;=T&lt;=100). Each of the next T lines consists of a single integer N (1&lt;=N&lt;=1000000), indicating the size of the way.

</p><h3>Output</h3>
<p>For each test case, output the last four digits of the number of ways of carpeting the 2xN way. If the answer involves fewer than 4 digits, print the entire number.<br>
<strong>Important Update - If the output of last four digits has leading zeros, print the output without the leading zeros</strong>


</p><h3>Example</h3>

<pre><b>Input:</b>
2
3
13

<b>Output:</b>
5
3465
</pre>