<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MDOSTAVA/en/">English</a></td>
<td width="50%"><a href="/problems/MDOSTAVA/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><p>&nbsp;</p>
<p>Little Ivica recently got a job delivering pizzas for the most popular  pizzeria in town.</p>
<p>At the start of his work day, he receives a list with the locations to  which he needs to deliver pizzas, inorder in which the locations are given.</p>
<p>The city is divided into R¡ÁC cells. The rows are numbered 1 through R,  columns 1 through C.</p>
<p>From every cell, it is possible to move to neighbouring cells to the  left and right. Moving up or down is only allowed in the first and last columns (columns 1 and C).</p>
<p>The pizzeria is in the top left corner (1, 1) and this is the location Ivica starts from. Ivica takes with him all the pizzas he will deliver that day  so he does not have to return to the pizzeria between deliveries or after the last delivery.</p>
<p>For each location in the city, Ivica knows how much time he will spend every  time he is in it (trying to get through the intersection, for example). Write a program that calculates the smallest amount of time for Ivica to  deliver all the pizzas.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line contains the integers R and C (1 ¡Ü R ¡Ü 2000, 1 ¡Ü C ¡Ü 200), the dimensions of the city.</p>
<p>Each of the following R lines contains C integers. These are the times  Ivica spends every time he enters a location. The times will be integers  between 0 and 5000, inclusive.</p>
<p>The next line contains an integer D (1 ¡Ü D ¡Ü 200 000), the number of  pizza deliveries that day. (No, it's not unrealistically large at all.) Each of the following D lines contains two integers A and B (1 ¡Ü A ¡Ü R,  1 ¡Ü B ¡Ü C), the location to which a pizza must be delivered. The  pizzas are given in the order in which they must be delivered. No location will be given twice in a row.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>Output the smallest amount of time for Ivica to deliver all the pizzas.</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>input
3 3
1 8 2
2 3 2
1 0 1
3
1 3
3 3
2 2
output
17

input
2 5
0 0 0 0 0
1 4 2 3 2
4
1 5
2 2
2 5
2 1
output
9
</pre>
<p>In the first example, the shortest path goes through the following locations: (1, 1), (2, 1), (3, 1), (3, 2), (3, 3), (2, 3), (1, 3), (2, 3), (3, 3), (2, 3) and (2, 2). The locations in bold show where Mirko made deliveries. The total time  for the deliveries is 1+2+1+0+1+2+2+2+1+2+3=17.</p>