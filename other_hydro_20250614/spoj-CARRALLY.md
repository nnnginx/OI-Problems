<p>In an attempt to demonstrate the practicality of electric cars, ElecCarCo is sponsoring a cross-country road rally. There are n charging stations for the rally where cars may check in and charge their batteries.</p>
<p>The rally may require multiple days of travel. Each car can travel four hours (240 minutes) between charges. A car must be plugged into a charger for two minutes for each minute of travel time. Cars start the rally at noon on the first day, fully charged. Cars are permitted remain at a station even after they are fully charged.</p>
<p>It is only possible to drive directly between select pairs of stations. Variations in traffic conditions, road conditions, availability of HOV lanes, etc., result in different travel times along each route depending upon the time of day at which travel along that route begins. All roads are two-way, and the prevailing conditions affect travel in both directions.</p>
<p>The winner is the first car to reach checkpoint n-1, starting form checkpoint 0. Other than the starting and ending conditions, cars may pass through the stations in any order, and need not visit all stations to complete the course.</p>
<p>Write a program to determine the earliest time, expressed as the total number of minutes elapsed since the start of the rally, at which a car could reach the final checkpoint.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There will be several test cases in the input. Each test case starts with a line containing n</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(1¡Ün¡Ü500), the number of stations, and m (1¡Üm¡Ü1,000), the number of connecting road</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">segments.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This is followed by m blocks, each block describing one road segment. A road segment</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">block has the following structure:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each block begins with a single line containing two integers, a and b (0¡Üa,b¡Ün-1, a¡Ùb).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">These numbers are the two checkpoints connected by that segment. The connections</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">are undirected: a segment permitting travel from station a to station b will also allow</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">travel from station b to station a.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This is followed by from one to twenty 'travel lines' describing travel times. Each of the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">travel lines contains 3 numbers: Start, Stop, (0¡ÜStart&lt;Stop¡Ü1,439), and Time</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(0&lt;Time&lt;1,000). Start and Stop are the time of day (expressed in minutes since</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">midnight) described by this line, and Time is the travel time, in minutes, required to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">traverse this road segment if travel begins at any time in the range [Start..Stop],</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">inclusive. The first travel line in a block will have a start time of 0 (midnight, or 00:00).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The final travel line in a block will have a stop time of 1439 (i.e., 23:59, or 1 less than 24&nbsp;</div>
<p>There will be several test cases in the input. Each test case starts with a line containing n (1¡Ün¡Ü500), the number of stations, and m (1¡Üm¡Ü1,000), the number of connecting road segments. This is followed by m blocks, each block describing one road segment. A road segment block has the following structure: Each block begins with a single line containing two integers, a and b (0¡Üa,b¡Ün-1, a¡Ùb). These numbers are the two checkpoints connected by that segment. The connections are undirected: a segment permitting travel from station a to station b will also allow travel from station b to station a. This is followed by from one to twenty 'travel lines' describing travel times. Each of the travel lines contains 3 numbers: Start, Stop, (0¡ÜStart&lt;Stop¡Ü1,439), and Time (0&lt;Time&lt;1,000). Start and Stop are the time of day (expressed in minutes since midnight) described by this line, and Time is the travel time, in minutes, required to traverse this road segment if travel begins at any time in the range [Start..Stop], inclusive. The first travel line in a block will have a start time of 0 (midnight, or 00:00). The final travel line in a block will have a stop time of 1439 (i.e., 23:59, or 1 less than 24 hours times 60 minutes). Adjacent travel lines in the input will be arranged in order, and the start time of any line after the first is one higher than the stop time of the preceding line. The travel lines will cover all times from 00:00 to 23:59. Input will end with a line with two 0s. All test cases will describe a course that can be completed by the cars.</p>
<h3>Output</h3>
<p>For each test case, output a single integer representing the smallest number of minutes needed to complete the rally. Output no spaces, and do not separate answers with blank lines.</p>
<h3>Example Input</h3>
<pre>4 4
0 1
0 1439 100
0 2
0 1439 75
1 3
0 720 150
721 824 100
825 1000 75
1001 1439 150
2 3
0 1439 150
3 2
0 1
0 10 200
11 1439 300
1 2
0 10 200
11 1439 300
4 3
0 1
0 719 500
720 1439 240
1 2
0 964 500
965 1439 2
2 3
0 971 500
972 1439 3
0 0</pre>
<h3>Example Output</h3>
<pre>180
2360
255</pre>
<p>&nbsp;</p>