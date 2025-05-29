<p>   </p>
<table style="border: 1px solid #2dd254; width: 100%; background-color: #d5d229;" border="1">
<tbody>
<tr>
<td style="text-align: center;" width="50%"><a href="/problems/MROADS/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/MROADS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>The traffic network in a country consists of N cities (labeled with integers 1 to N) and N-1 roads connecting the cities. There is a unique path between each pair of different cities.</p>
<p><br>Because of the many years of lazy maintenance the roads are pretty damaged and for each road two numbers A and B are known ¨C the integer A represents the current time (in seconds) needed to travel along the road, and the integer B represents the smallest possible time (in seconds) needed to travel along this road if we repair all the damage.</p>
<p><br>We want to invest a certain amount of money into road repair. For a particular road, the result will be proportional to the amount of invested money. For each euro invested in some road, the time needed to travel along that road will be reduced by one second (the amount of money invested in some road has to be an integer). The travel time cannot be reduced beyond the smallest possible time B described above.</p>
<p><br>We are given a certain amount of money. We want to distribute this money along different roads in such a way that the time needed to travel from the city 1 to the most distant city (after all the repairs) is as small as possible.</p>
<p><br>Write a program that will find this smallest time.</p>
<h3>Input</h3>
<p>The first line of input contains two integers N and K, 2 ¡Ü N ¡Ü 100 000, 0 ¡Ü K ¡Ü 1 000 000, the number of cities and the total amount of money (in euros).</p>
<p><br>Each of the next N-1 lines contains four integers X, Y, A and B, 0 ¡Ü B ¡Ü A ¡Ü 10 000. It means that there is a road between cities X and Y, with the numbers A and B representing the current time and the minimum time as described above.</p>
<h3>Output</h3>
<p>The first and only line of output should contain a single integer ¨C the minimum time from the task description.</p>
<h3>Sample</h3>
<pre>input <br>&nbsp;<br>3 200 <br>1 2 200 100 <br>2 3 450 250 <br>&nbsp;<br>output <br>&nbsp;<br>450<br><br>input <br>&nbsp;<br>5 11 <br>1 2 10 5 <br>1 3 3 2 <br>1 4 9 6 <br>3 5 7 3 <br>&nbsp;<br>output <br>&nbsp;<br>6<br><br>input <br>&nbsp;<br>11 12 <br>1 2 7 5 <br>1 3 20 15 <br>2 4 10 8 <br>2 5 5 3 <br>2 6 6 2 <br>4 7 3 0 <br>4 8 7 2 <br>5 9 8 4 <br>5 10 9 8 <br>5 11 6 5 <br>&nbsp;<br>output <br>&nbsp;<br>17</pre>
<p> </p>