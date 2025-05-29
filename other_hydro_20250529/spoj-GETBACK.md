<p>Somewhere deep in a desert lives a small, completely forgotten tribe N'Gubara. All the men, women and children of the tribe live with a few camels in the N'Gubara oasis (the N'Gubara people don't have great creativity when it comes to geography names). These poor people have only the N'Gubara well, a few acres of irrigated land and the N'Gubara cave. Yes, the cave. </p>

<p>You do not remember exactly how you have come to N'Gubara. Maybe your car broke when you travelled across the desert. Maybe you jumped out of an airplane. Maybe you were brought here by Martians. But this does not matter now. You know that you are here, pretty far from any civilization. And you desperately want to go home. </p>

<p>The only possibility how to get home is to walk across the desert to Desertville, the closest city. You have to use paths in the desert shown in your map. Each such path connects two restpoints. The N'Gubara oasis and Desertville are also considered to be restpoints. You can walk, but you need water. For each mile travelled, you have to drink one unit of water. You are able to carry at most C units of water at once. Thus, you can never walk more than C miles without replenishing your water supply. The shortest way to Desertville is probably much longer than C miles. It would thus seem that you will stay in N'Gubara forever, but there's a trick: at the end of each path, there is a restpoint with an empty water reservoir. You can transport water into a reservoir from N'Gubara or from other reservoirs where you stored some water previously. You can then use the stored water later on (the water doesn't evaporate). Of course, you can take only as much water from any reservoir as you brought into it. You may use as much water from the N'Gubara oasis as you need, but since water is very valuable in the desert, you promised that you will use only the minimal amount needed for your return to Desertville. In this task, we want you to compute the minimal amount of water you need. </p>

<h3>Input file specification</h3>
<p>Input contains several test cases, the number of them is given in the very first line.</p>
<p>The first line contains three integers N, M and C, where N is the number of the restpoints, M is the number of the paths and C is your carrying capacity. M lines follow, each describing one path on the map. Each line contains three numbers x, y and l, where x and y are the restpoints joined by a path and l is the length of that path in miles. The restpoints are numbered from 1 to N, where restpoint 1 is the N'Gubara oasis and restpoint N is Desertville. </p>
<p>You may assume all the numbers in the input file are non-negative integers less than 100.</p>

<h3>Output file specification</h3>
<p>For each test case:</p>
<p>Your output file should contain a single integer - the minimum amount of water needed for you to get from N'Gubara to Desertville. If there is no possibility how to get to Desertville with your current carrying capacity C, you should output the number -1. </p>

<h3>Example</h3>
<pre><b>Input file:</b>
1
9 10 25
1 2 3
2 3 12
3 4 4
3 5 9
4 9 13
5 9 5
2 6 10
6 7 10
7 8 10
8 9 10

<b>Output file:</b>
65
</pre>
<p>Note: You can get to Desertville as follows: first you take 25 units of water from N'Gubara, go to restpoint 2, leave there 19 units in the reservoir and go back to N'Gubara. Then you repeat this trip, bringing additional 19 units to restpoint 2. Last, you take 15 units from N'Gubara to restpoint 2. Now you have 19+19+12 = 50 units of water here. You take a round trip to point 3 and back, leaving there 1 unit of water. Now you take all water left from point 2, go to point 3, take the one unit from point 3 (now you have 25-12+1=14 units) and go via restpoint 5 to Desertville. </p>