<p>&nbsp;</p>
<p>Seraph is a smart boy who, one day at the time of his birthday he was wearing a lot of lights for the event. The number of lights is installed for as many as N, which are numbered 1 through N. lights are connected to a controller that has 4 buttons. Each button functions as follows:</p>
<p>1. if this button is pressed, then all light will change the state from OFF to ON or from ON to OFF</p>
<p>2. if this button is pressed, then the odd-numbered light will change its state</p>
<p>3. if this button is pressed, then the even-numbered light will change its state</p>
<p>4. if this button is pressed, all lights are numbered 3K +1 will change its state</p>
<p>In the controller, there are counter C that count number of button will be pressed. when the initial state, the state of all the lights are ON and the counter C is set to 0. After that you will be given information of light at the end of the show, and you have to count how many kinds of configuration according to the information provided.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Seraph is a smart boy who, one day at the time of his birthday he was wearing a lot of lights for the event. The number of lights is installed for as many as N, which are numbered 1 through N. lights are connected to a controller that has 4 buttons. Each button functions as follows:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1. if this button is pressed, then all light will change the state from OFF to ON or from ON to OFF</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2. if this button is pressed, then the odd-numbered light will change its state</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3. if this button is pressed, then the even-numbered light will change its state</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4. if this button is pressed, all lights are numbered 3K +1 will change its state</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">
<p>In the controller, there are counter C that count number of button will be pressed. when the initial state, the state of all the lights are ON and the counter C is set to 0. After that you will be given information of light at the end of the show, and you have to count how many kinds of configuration according to the info</p>
<p>rmation ahdadhprovided.</p>
</div>
<p><strong>Input</strong></p>
<p>The first line containing N (10 &lt;= N &lt;= 100) that indicates number of lamps. The second line is C (1 &lt;= C &lt;= 1000) that indicate the final value of counte. The third line is lists the number of ON lights at the end of the show, each number separated by a space and the end of the line given the value -1. The fourth line is lists the number of OFF light at the end of the show, each number separated by a space and the end of the line given the value -1.</p>
<h3>Output</h3>
<p>configurations are possible at the end of the event. There should be no repetitive configuration and output must be in lexicographical. If there is no configuration, print "Impossible".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10
1
-1
7 -1

<strong>Output:</strong>
0000000000
0101010101
0110110110<span style="white-space: normal;">
</span></pre>
<pre>Explanation :</pre>
<pre>There is 10 lamps in that event and you have to pressed the button once, and at the end of event, lamp number 7 must be OFF.</pre>
<pre>0 mean that lamp is OFF, 1 mean that lamp is ON&nbsp;</pre>