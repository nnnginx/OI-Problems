<p>The next MechaGodzilla invasion is on its way to Earth. And once again, Earth will be the battleground for an epic war.

</p><p>MechaGodzilla's army consists of many nasty alien monsters, such as Space Godzilla, King Gidorah, and MechaGodzilla herself.

</p><p>To stop them and defend Earth, Godzilla and her friends are preparing for the battle.</p>

<h3>Problem specification</h3>

<p>Each army consists of many different monsters. Each monster has a strength that can be described by a positive integer. (The larger the value, the stronger the monster.) 

</p><p>The war will consist of a series of battles. In each battle, the weakest of all the monsters that are still alive is killed. 

</p><p>If there are several weakest monsters, but all of them in the same army, one of them is killed at random. If both armies have at least one of the weakest monsters, a random weakest monster of MechaGodzilla's army is killed. 

</p><p>The war is over if in one of the armies all monsters are dead. The dead army lost, the other one won. 

</p><p>You are given the strengths of all the monsters. Find out who wins the war.</p>

<h3>Input specification</h3>

<p>The first line of the input file contains an integer T specifying the number of test cases. Each test case is preceded by a blank line. 

</p><p>Each test case starts with line containing two positive integers NG and NM �C the number of monsters in Godzilla's and in MechaGodzilla's army. Two lines follow. The first one contains NG positive integers �C the strengths of the monsters in Godzilla's army. Similarly, the second one contains NM positive integers �C the strengths of the monsters in MechaGodzilla's army.</p>

<h3>Output specification</h3>

<p>For each test case, output a single line with a string that describes the outcome of the battle. 

</p><p>If it is sure that Godzilla's army wins, output the string "Godzilla". 

</p><p>If it is sure that MechaGodzilla's army wins, output the string "MechaGodzilla".

</p><p>Otherwise, output the string "uncertain".</p>

<h3>Example</h3>
<pre><b>input:</b>
2

1 1
1
1

3 2
1 3 2
5 5

<b>output:</b>
Godzilla
MechaGodzilla
</pre>
<h3>Hint</h3>
<p>In the first test case, there are only two monsters, and they are equally strong. In this situation, MechaGodzilla's monster is killed and the war ends.

</p><p>In the second test case, the war will consist of three battles, and in each of them one of Godzilla's monsters dies.

</p><p>For all the test cases, <b>int</b> in C/C++/Java or <b>longint</b> in Pascal is enough.</p>