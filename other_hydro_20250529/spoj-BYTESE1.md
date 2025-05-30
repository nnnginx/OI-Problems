<p>LUCIUS�� DUNGEON (5 points)

There are a set of rooms in a dungeon, arranged in an M �� N rectangular grid. In one of the rooms, evil Lucius Malfoy has imprisoned Hermione, owing to his hatred towards the mudbloods. The noble Harry potter is on his way to rescue Hermione. Harry potter starts in the room at the top left corner of the grid, which is labeled (1,1). Each room contains some guards. It takes some time for Harry potter to kill all the guards in the room he is in. The time taken to kill the guards varies from room to room. Once he has killed all the guards in a room, he can move on to any one of its neighbors by going left, right, up or down, provided, of course, that there is a neighboring room in the corresponding direction. He cannot move diagonally.<br>Lucius Malfoy, knowing that Harry Potter is on his way, has set a time bomb that will kill Hermione after T seconds. You will be given the position of Hermione, the time left for the bomb to go off and the time it takes for Harry to kill the guards in each of the rooms in the dungeon. Your task is to determine if it is possible for Harry to reach Hermione and save her by defusing the bomb before the T seconds expire.
For example, suppose the dungeon is described by the following grid of numbers where the numbers start from (1,1):<br>
2 3 2<br>
2 5 1<br>
5 3 1<br>
3 1 1<br>
The number at position (i,j) indicates the time taken for Harry Potter to overpower the guards in room (i,j). Suppose Hermione is in the room at position (4,2). If T = 10. There is no way Harry Potter can reach Hermione in time. However, if M = 15, Harry Potter can reach Hermione with 4 seconds to spare, as follows. Starting from (1,1), he moves right to (1,2) and then (1,3), comes down all the way to (4,3) and then moves to (4,2). This takes 11 seconds (note that he must also overpower the guard in the room where Hermione is incarcerated). You can check that he cannot reach Hermione with more than 4 seconds to spare by any route.<br>Note: If Harry reaches Hermione at exactly ��T�� seconds from the start then the answer is ��YES�� with 0 seconds to spare.


</p><h3>Input</h3>
<p>The first line consists of the number of test cases K (1&lt;=K&lt;=20). In each test case, the first line contains two integers M and N indicating the number of rows and columns in the rectangular dungeon(1 �� M,N�� 100). Next M lines contain N integers (single digits only). The jth integer on ith line is the time taken to overpower the guards at room (i,j). The last line in each test case, contains three integers a, b and T, where (a,b) is the position of the cell where Hermione is held and T is the amount of time before the bomb goes off.

</p><h3>Output</h3>
<p>For each of the test case, if it is not possible for Harry Potter to save Hermione then print NO. Otherwise, print two lines. The first line should say YES. The second line should contain a single integer indicating the maximum possible time to spare when Harry Potter rescues the Hermione.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4 3 
2 3 2
2 5 1
5 3 1
3 1 1
4 2 15
2 2
1 2
1 1
2 2 2

<b>Output:</b>
YES
4
NO
</pre>