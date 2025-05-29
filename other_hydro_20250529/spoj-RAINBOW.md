<p>Mr.Raju and his extended family are on vacation in Chennai. They visit MGM and see the Rainbow ride. They want to enjoy the ride. However, there are some problems.
</p><p>
Each person in the family likes some other people in the family. Each person insists that he or she will go on the ride only if all the people whom that person likes and all the people who like that person also go on the ride. If someone doesn't like anyone and no one likes him, he may come for the ride.
</p><p>
You have been roped in to solve this dilemma. Given the weight of the each person in the family, and the list of people they like, and the maximum weight that the Rainbow can bear safely, calculate the maximum number of people in the family who can go on the rainbow. 

</p><h3>Input</h3>
<p> There will be multiple test cases in the input. For our convenience the family members are numbered from 1 to n. Each test case begins with a line containing two   integers <b>n</b> ( 1 �� n �� 1000 ) and <b>C</b> ( 0 �� C �� 1000 ), where n is the number of people in the family and C the maximum capacity of the ride in kilograms.</p>
<p>
The next line contains n space separated integers with the <b>i</b>th integer giving the weight of the <b>i</b> th family member. These weights are positive and less than or equal to 200 kilograms. Then n lines follow. Each line contains a sequence of integers separated by spaces. The first integer <b>k<sub>i</sub></b> gives the number of people in the family person <b>i</b> likes, followed by the persons <b>i</b> likes. An empty line separates each test case. The end of input is indicated by n=0 and C=0 and it should not be processed.There are atmost 50 test cases.

</p><h3>Output</h3>
<p>For each test case output on a separate line the maximum number of persons that can take the ride under the given conditions.

</p><h3>Example</h3>

<pre><b>Input:</b>
5 200
50 50 50 50 50
1 2
1 3
0
1 5
1 4

3 200
100 100 100
1 2
1 3
1 1

0 0

<b>Output:</b>
3
0
</pre>