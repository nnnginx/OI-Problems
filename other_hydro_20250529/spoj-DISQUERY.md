<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td style="text-align: center;" width="50%"><a href="/problems/DISQUERY/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/DISQUERY/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p><br>
</p><p>The traffic network in a country consists of N cities (labeled with integers from 1 to N) and N-1 roads connecting the cities. There is a unique path between each pair of different cities, and we know the exact length of each road. </p>
<p>Write a program that will, for each of the K given pairs of cities, find the length of the shortest and the length of the longest road on the path between the two cities. </p>

<h3 style="text-align: center;">Input</h3>
<p>The first line of input contains an integer N, 2 ¡Ü N ¡Ü 100 000. Each of the following N-1 lines contains three integers A, B and C meaning that there is a road of length C between city A and city B. </p>
<p>The length of each road will be a positive integer less than or equal to 1 000 000. <br>
The next line contains an integer K, 1 ¡Ü K ¡Ü 100 000. Each of the following K lines contains two different integers D and E ¨C the labels of the two cities constituting one query. </p>

<h3 style="text-align: center;">Output</h3>
<p>Each of the K lines of output should contain two integers ¨C the lengths from the task description for the corresponding pair of the cities. </p>

<h3 style="text-align: center;">Sample</h3>
<pre>input:

5
2 3 100
4 3 200
1 5 150
1 3 50
3
2 4
3 5
1 2

output:

100 200
50 150
50 100

input:

7
3 6 4
1 7 1
1 3 2
1 2 6
2 5 4
2 4 4
5
6 4
7 6
1 2
1 3
3 5

output:

2 6
1 4
6 6
2 2
2 6</pre>

<br>