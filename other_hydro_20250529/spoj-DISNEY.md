<div style="text-align: left; margin: 10px 0px;"><div style="float: right; margin: 0px 0px 3px 10px;"><img src="/content/crazyb0y:DISNEY.jpg" width="250"></div><span>


<blockquote>
<i><p>Disney's FastPass is a virtual queuing system created by the Walt Disney Company. First introduced in 1999 (thugh the idea of a ride reservation system was first introduced in world fairs), FastPass allows guests to avoid long lines at the attractions on which the system is installed, freeing them to enjoy other attractions during their wait. The service is available at no additional charge to all park guests.</p>
<p>--- Wikipedia</p>
</i>
</blockquote>

<p>Disneyland is a large theme park with plenties of entertainment facilities, also with a large number of tourists. Normally, you need to wait for a long time before getting the chance to enjoy any of the attractions. The FastPass is a system allowing you to pick up FastPass-tickets in some specific position, and use them at the corresponding facility to avoid long lines. With the help of the FastPass System, one can arrange his/her trip more efficiently.</p>

<p>You are given the map of the whole park, and there are some attractions that you are interested in. How to visit all the interested attractions within the shortest time?</p>
</span></div>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 �� <b>T</b> �� 25), indicating the number of test cases.</p>

<p>Each test case contains several lines.
The first line contains three integers <b>N</b>, <b>M</b>, <b>K</b> (1 �� <b>N</b> �� 50, 0 �� <b>M</b> �� <b>N</b>(<b>N</b>-1)/2, 0 �� <b>K</b> �� 8), indicating the number of locations(starting with 1, and 1 is the only gate of the park where the trip must be started and ended), the number of roads and the number of interested attractions.</p>

<p>The following <b>M</b> lines each contains three integers <b>A</b>, <b>B</b>, <b>D</b> (1 �� <b>A</b>, <b>B</b> �� <b>N</b>, 0 �� <b>D</b> �� 10<sup>4</sup>) which means it takes <b>D</b> minutes to travel between location <b>A</b> and location <b>B</b>. </p>

<p>The following <b>K</b> lines each contains several integers <b>P</b><sub><i>i</i></sub>, <b>T</b><sub><i>i</i></sub>, <b>FT</b><sub><i>i</i></sub>, <b>N</b><sub><i>i</i></sub>, <b>F</b><sub><i>i</i>,1</sub>, <b>F</b><sub><i>i</i>,2</sub> ...  <b>F</b><sub><i>i</i>,<b>N</b><sub><i>i</i></sub>-1</sub>, <b>F</b><sub><i>i</i>,<b>N</b><sub><i>i</i></sub></sub>, (1 �� <b>P</b><sub><i>i</i></sub>, <b>N</b><sub><i>i</i></sub>, <b>F</b><sub><i>i</i>,<i>j</i></sub> �� <b>N</b>, 0 �� <b>FT</b><sub><i>i</i></sub> �� <b>T</b><sub><i>i</i></sub> �� 10<sup>4</sup>), which means the i-th interested attraction is placed at location <b>P</b><sub><i>i</i></sub> and there are <b>N</b><sub><i>i</i></sub> locations <b>F</b><sub><i>i</i>,1</sub>, <b>F</b><sub><i>i</i>,2</sub> ... <b>F</b><sub><i>i</i>,<b>N</b><sub><i>i</i></sub></sub> where you can get the FastPass for the <i>i</i>-th attraction. If you come to the <i>i</i>-th attraction with its FastPass, you need to wait for only <b>FT</b><sub><i>i</i></sub> minutes, otherwise you need to wait for <b>T</b><sub><i>i</i></sub> minutes.</p>

<p>You can assume that all the locations are connected and there is at most one road between any two locations.
Note that there might be several attractions at one location.</p>


<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is the minimum time of the trip.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4 5 2
1 2 8
2 3 4
3 4 19
4 1 6
2 4 7
2 25 18 1 3
4 12 6 1 3
4 6 2
1 2 5
1 4 4
3 1 1
3 2 1
3 4 1
2 4 10
2 8 3 1 4
4 8 3 1 2

<b>Output:</b>
Case #1: 53
Case #2: 14
</pre>