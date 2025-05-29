<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MELE3/en/">English</a></td> 
<td width="50%"><a href="/problems/MELE3/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
Solitaire has N elevators. Each elevator are connecting exactly two 
floors and it does not stop on the floors between that two floors 
The speed of all the elevators are the same, 5 seconds to pass one floor. </p><p>
On the beginning, each elevator is in its lower position and they 
are starting cruising to the upper floor. After some elevator come 
to its upper position, it  immediatly starts to go back to its lower 
position, and so on... </p><p>
Mirko is on the  first (the lowest) floor and he wants as quick as 
possible come to the  top of the solitaire. He can change elevators 
only on the floors that are common to both elevators, and if the other 
elevator is in that moment on that floor, that change 
does not take 
any time. </p><p>
Write a program that will calculate minimal time in which Mirko can get 
to the top of the solitaire.
</p><p>
</p><h3>Input</h3>
<p></p><p>
In the first line of the input file there are two integers K 
and N, separated with space, number of floors in solitaire and 
number of elevators, 2 ¡Ü K ¡Ü 1000, 1 ¡Ü N ¡Ü 50000. </p><p>
In each of the next N lines there are description of one elevator, 
two integers A and B, separated with space, 1 ¡Ü A &lt; B ¡Ü K, means that 
elevator is travelling between floors A and B. </p><p>
There are no two different elevators that travels between same floors. </p><p>
Note: input data will guarantee that solution will always exists. 
</p><p>
</p><h3>Output</h3>
<p></p><p>
In the only line of output file write minimal time (in seconds) from 
the text above. 
</p><p>
</p><h3>Sample</h3>
<pre>liftovi.in 
 
10 4 
1 5 
5 10 
5 7 
7 10 
 
liftovi.out 
 
45 

liftovi.in 
 
10 3 
1 5 
3 5 
3 10 
 
liftovi.out 
 
105 

liftovi.in 
 
20 5 
1 7 
7 20 
4 7 
4 10 
10 20 
 
liftovi.out 
 
150 

</pre>