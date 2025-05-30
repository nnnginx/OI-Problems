<p>Millions of years ago massive fields of ice carved deep grooves in the mountains of Norway. The sea filled these grooves with water. The Norwegian people call them fjords. This landscape of mountains and water is beautiful, but it makes traveling difficult. The usual scheme is: drive some kilometers, wait for a ferry, cross a fjord with the ferry, drive some more kilometers, and so on until the destination has been reached. To reach a destination as early as possible, most people have the following strategy: drive as fast as allowed (the maximum speed is 80 km/h) to the next ferry, and wait until it goes. Repeat until the destination has been reached. 
</p><p>Since driving fast requires more fuel than driving slow, this strategy is both expensive and harmful to the environment. The new generation of cruise control systems is designed to help. Given the route you want to go, these systems will gather information about the ferries involved, calculate the earliest possible time of arrival at the final destination, and calculate a driving scheme that avoids driving faster than needed. The systems will calculate your road speed so that you board the next ferry the moment it leaves. 
</p><p>Given a route (a sequence of road-pieces and crossings with ferries), you must write a program to calculate the minimal time it takes to complete this route. Moreover, your program must find a driving scheme such that the maximal driving speed at any point during the trip is as small as possible. </p>
<h3>Input</h3>
<p>The input file contains one or more test cases. Each test case describes a route. A route consists of several sections, each section being either a piece of road or a crossing. The first line in the description contains a single number s (s &gt; 0), which is the number of sections in the route. The next s lines contain the descriptions of the sections. Every line describing a section starts with two names: the place of departure and the place of arrival, followed by either the word ��road�� or the word ��ferry�� indicating what kind of section it is. If the section is a road, its length (a positive integer) is given in km. For example: </p>
<p><i>Dryna Solholmen road 32</i></p>
<p>Lines describing ferry sections have more information. Following the word ��ferry��, the duration of the ferry crossing, in minutes (a positive integer) is given. This is followed by the frequency f (f &gt; 0) of the ferry, that is, the number of times the ferry departs in a single hour. The next f integers give the departure times of the ferry, in ascending order. For example: </p>
<p><i>Manhiller Fodnes ferry 20 2 15 35 </i></p>
<p>The ferry travels from Manhiller to Fodnes in 20 minutes, and it leaves twice an hour (on 0h15, 0h35, 1h15, 1h35,��). The beginning of the entire trip always starts at a full hour. The sections in a route are consecutive, that is, if a section goes from A to B then the next section starts at B. Every route in the input can be traveled in no more than 10 hours. 
</p><p>The input is terminated by the number zero on a line by itself.
</p><h3>Output</h3>
<p>Output for each test case is a single line containing three items. The first item is the test case number. The second is the total travel time for an optimal scheme in the form hh:mm:ss. The third item is the maximal road speed in an optimal scheme rounded to two digits to the right of the decimal point. 
</p><p>Place a blank line after the output of each test case.</p>
<h3>Example</h3>
<pre><b>Input:</b>
1
Bygd Bomvei road 7
2
Ferje Overfarten ferry 20 2 5 25
Overfarten Havneby ferry 30 3 10 30 50
5
Begynnelse Brygge road 30
Brygge Bestemmelse ferry 15 4 10 25 40 55
Bestemmelse Veiskillet road 20
Veiskillet Grusvei road 25
Grusvei Slutt ferry 50 1 10
0

<b>Output:</b>
Test Case 1: 00:05:15 80.00

Test Case 2: 01:00:00 0.00

Test Case 3: 03:00:00 45.00

</pre>