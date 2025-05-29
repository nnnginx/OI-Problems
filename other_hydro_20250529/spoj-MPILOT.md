<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MPILOT/en/">English</a></td> 
<td width="50%"><a href="/problems/MPILOT/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Charlie acquired airline transport company and to stay in business he needs to lower the expenses by 
any means possible. 
There are N pilots working for his company (N is even) and N/2 plane crews needs to be made. A 
plane crew consists of two pilots - a  captain and his  assistant. A captain must be older than his 
assistant. Each pilot has a contract granting him two possible salaries - one as a captain and the other as 
an assistant. A captain's salary is larger than assistant's for the same pilot. However, it is possible that an 
assistant has larger salary than his captain.  
Write a program that will compute the minimal amount of money Charlie needs to give for the pilots' 
salaries if he decides to spend some time to make the optimal (i.e. the cheapest) arrangement of pilots 
in crews. 
 
</p><p>
</p><h3>Input</h3>
<p></p><p>
The first line of input contains integer N, 2 ¡Ü N ¡Ü 10,000, N is even, the number of pilots working for 
the Charlie's company. 
The next N lines of input contain pilots' salaries. The lines are sorted by pilot's age, the salaries of the 
youngest pilot are given the first. Each of those N lines contains two integers separated by a space 
character, X i Y, 1 ¡Ü Y &lt; X ¡Ü 100,000, a salary as a captain (X) and a salary as an assistant (Y). 
</p><p>
</p><h3>Output</h3>
<p></p><p>
The first and only line of output should contain the minimal amount of money Charlie needs to give 
for the pilots' salaries. 
 
</p><p>
</p><h3>Sample</h3>
<pre>input 
4 
5000 3000 
6000 2000 
8000 1000 
9000 6000 
 
output 
19000 

input 
6 
10000 7000 
9000 3000 
6000 4000 
5000 1000 
9000 3000 
8000 6000 
 
output 
32000 


</pre>