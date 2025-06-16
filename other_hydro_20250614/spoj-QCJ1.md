<p>In this problem your task is to program a robot that will output some data about a terrain after traversing it. Input will be in the form a 2D picture containing only 4 types of characters :-</p>
<pre><li> '/' :  Forward slash, indicating ascent</li><li> '\' :  Backward slash, indicating descent</li><li> '_' :  Underscore, denoting horizontal plane</li></pre>
<p>Additionally there will be only SPACE (Ascii value = 32) charecters. ( Refer the below figure).</p>
<p>The robot starts its journey at bottom left corner of the terrain and after traversing stops at the bottom right corner. Also note that the robot will always start and end at the SAME LEVEL.</p>
<p>Given the picture as input you will have to output 2 things. The "Total Walk Distance" i.e, the total length of the path and the type of steps taken to complete the Journey. For the sake of simplification we will assume that each charecter('/' , '\' &amp; '_') has length = 1.</p>
<p>Now Consider the following example:</p>
<pre>		   _<br>		  / \/\<br>		 /     \<br>		/       \<br></pre>
<p>The robot starts at the bottom left corner and takes the following path:</p>
<pre><li> Ascends 3 steps</li><li> Moves forward by 1 step</li><li> Descends 1 step</li><li> Ascends 1 step</li><li> Descends 3 steps</li></pre>
<p>and robot ends it journey at bottom right corner (At the same level). The Total Walk Distance = 9.</p>
<h3>Input</h3>
<p>First line of input will be an integer N (N&lt;20). The next line will be an empty. Then exactly N lines follow describing the terrain.<br> You can assume the following for the input (terrain).</p>
<pre><li> Input will contain only four types of characters (" ","_","/","\").</li><li> The terrain will start and end at the same level.</li><li> Each line is guarenteed to have atleast one non white space charecter.</li><li> Maximum width of any line wont be larger than 200.</li><li> There will be no trailing white spaces.</li></pre>
<h3>Output</h3>
<p>First line of output should be the Total Walk Distance followed by the description the the the terrain. Each line must be ONE of the following</p>
<pre><li> Up xx steps</li><li> Down xx steps</li><li> Walk xx steps</li></pre>
<p>Where xx is an integer.<br> Refer Examples for exact specification.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br><br>  /\<br> /  \<br>/    \<br><br><strong>Output:</strong><br>Total Walk Distance = 6<br>Up 3 steps<br>Down 3 steps<br><br></pre>
<pre><strong>Input:</strong><br>2<br><br> _____  ___<br>/     \/   \<br><br><br><strong>Output:</strong><br>Total Walk Distance = 12<br>Up 1 steps<br>Walk 5 steps<br>Down 1 steps<br>Up 1 steps<br>Walk 3 steps<br>Down 1 steps<br><br></pre>
<pre><strong>Input:</strong><br>5<br><br>        _<br>   /\__/ \<br>  /       \<br> /         \/\_<br>/              \<br><br><strong>Output:</strong><br>Total Walk Distance = 16<br>Up 4 steps<br>Down 1 steps<br>Walk 2 steps<br>Up 1 steps<br>Walk 1 steps<br>Down 3 steps<br>Up 1 steps<br>Down 1 steps<br>Walk 1 steps<br>Down 1 steps<br><br></pre>