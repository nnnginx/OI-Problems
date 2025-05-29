<p>Eefun is a nomad who like to explore dungeons. On each dungeons, there's a valuable treasure waiting for him. However, Eefun should pass some obstacles to get the treasure.</p>
<p>In the dungeon, there are N doors which moves every second. These doors have width equal one and the dungeon has M width. When Eefun enters the dungeon (pass the first door), the timer start and the doors will start moving. The door will move to the right initially. When a door reach the end of the dungeons (at position M), then the door will change direction to left until reaching the leftmost position again (position 1). Eefun knows the initial position of all doors.</p>
<p>To pass a door, Eefun need to have same position with the door and he needs a second to pass a door. If next door has different position with Eefun, he can stay at the current position or move a position to the left or right.</p>
<p>After trying many dungeons, Eefun gets dizzy because he sees moving door everywhere. Therefore, he wants to know the minimum number of seconds to get the treasure. Eefun can obtain the treasure after he pass all the doors.&nbsp;</p>
<h3>Input</h3>
<p>First line contains 2 numbers, N and M.<br>Second line contains N numbers, the initial position of each doors.&nbsp;</p>
<h3>Output</h3>
<p>Output a single number, the minimum time Eefun needs to obtain the treasure.</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
3 5<br>1 4 3

<strong>Output 1:</strong>
5

<strong>Input 2:</strong>
5 5<br>1 1 1 1 1

<strong>Output 2:</strong>
18</pre>
<div style="border: 1px solid #ADC; background-color: #0cc; padding: 5px; margin-bottom: 10px;">
<h3>Explanation</h3>
For the first testcase, the initial doors are like picture below:<br><br>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|P****|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|-----|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|***P*|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|-----|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|**P**|&nbsp;</samp></p>
<span style="font-family: monospace; background-color: #00cccc;">First, Eefun will enter the dungeon at time = 1 and the doors will start moving<br></span><br>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|*P***|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|E----|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|****P|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|-----|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|***P*|</samp></p>
<div><span style="font-family: monospace;">Then, Eefun will move to the right 2 times</span><br><br>
<p style="font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; margin: 0px 0px 1.25em; padding: 0px; border: 0px; border-image-source: initial; border-image-slice: initial; border-image-width: initial; border-image-outset: initial; border-image-repeat: initial; font-size: 12px; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|***P*|</samp></p>
<p style="font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; margin: 0px 0px 1.25em; padding: 0px; border: 0px; border-image-source: initial; border-image-slice: initial; border-image-width: initial; border-image-outset: initial; border-image-repeat: initial; font-size: 12px; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|--E--|</samp></p>
<p style="font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; margin: 0px 0px 1.25em; padding: 0px; border: 0px; border-image-source: initial; border-image-slice: initial; border-image-width: initial; border-image-outset: initial; border-image-repeat: initial; font-size: 12px; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|**P**|</samp></p>
<p style="font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; margin: 0px 0px 1.25em; padding: 0px; border: 0px; border-image-source: initial; border-image-slice: initial; border-image-width: initial; border-image-outset: initial; border-image-repeat: initial; font-size: 12px; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|-----|<br></samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|***P*|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; border-image-source: initial; border-image-slice: initial; border-image-width: initial; border-image-outset: initial; border-image-repeat: initial; font-size: 12px; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp><span style="background-color: #00cccc;"><span style="font-size: small;">Then, Eefun will pass the second door which take one second.<br></span></span></samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|****P|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|-----|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|*P***|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|--E--|</samp></p>
<p style="margin: 0px 0px 1.25em; padding: 0px; border: 0px; font-size: 12px; font-family: 'Lucida Grande', Arial, Helvetica, sans-serif; vertical-align: baseline; line-height: 1.5em; color: #333333;"><samp>|**P**|</samp></p>
</div>
&nbsp;<span style="font-family: monospace; color: #333333;"><span style="line-height: 18px;">As Eefun already has same position with the last door, he can continue to the last door and take another second. His minimum time to pass all the doors are 1+2+1+1 = 5 seconds.</span></span></div>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>1 ¡Ü Position of each door ¡Ü M</li>
<li>1 ¡Ü N ¡Ü 1.000.000</li>
<li>1 ¡Ü M ¡Ü 10.000</li>
</ul>
</div>