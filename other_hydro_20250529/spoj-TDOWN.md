<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">As we all know, Bessie the cow likes nothing more than causing mischief on the farm.  To keep her from causing too much trouble, Farmer John decides to tie Bessie down to a fence with a long rope.  When viewed from above, the fence consists of N posts (1 &lt;= N &lt;= 10) that are arranged along vertical line, with Bessie's position (bx, by) located to the right of this vertical line.  The rope FJ uses to tie down Bessie is described by a sequence of M line segments (3 &lt;= M &lt;= 10,000), where the first segment starts at Bessie's position and the last ends at Bessie's position. No fence post lies on any of these line segments.  However, line segments may cross, and multiple line segments may overlap at their endpoints.</span></p>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">Here is an example of the scene, viewed from above:</span></span></p>
<p style="text-align: -webkit-left;"><span style="font-family: monospace;"><span style="font-size: 14px; white-space: pre-wrap;"><img src="./24631/file/on55zCvl.png" alt=""></span></span></p>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">To help Bessie escape, the rest of the cows have stolen a saw from the barn.  Please determine the minimum number of fence posts they must cut through and remove in order for Bessie to be able to pull free (meaning she can run away to the right without the rope catching on any of the fence posts).  All (x,y) coordinates in the input (fence posts, Bessie, and line segment endpoints) lie in the range 0..10,000.  All fence posts have the same x coordinate, and bx is larger than this value.</span></span></span></p>
<h3>Input</h3>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">* Line 1: Four space-separated integers: N, M, bx, by.</span></p>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">* Lines 2..1+N: Line i+1 contains the space-separated x and y         coordinates of fence post i.</span></span></p>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">* Lines 2+N..2+N+M: Each of these M+1 lines contains, in sequence, the         space-separated x and y coordinates of a point along the rope.         The first and last points are always the same as Bessie's         location (bx, by).</span></span></span></p>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;"><br></span></span></span></p>
<h3>Output</h3>
<p><span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">* Line 1: The minimum number of posts that need to be removed in order         for Bessie to escape by running to the right.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: monospace; font-size: 14px; text-align: -webkit-left; white-space: pre-wrap;">2 10 6 1</span></pre>
<pre>2 3</pre>
<pre>2 1</pre>
<pre>6 1</pre>
<pre>2 4</pre>
<pre>1 1</pre>
<pre>2 0</pre>
<pre>3 1</pre>
<pre>1 3</pre>
<pre>5 4</pre>
<pre>3 0</pre>
<pre>0 1</pre>
<pre>3 2</pre>
<pre>6 1</pre>
<pre><span style="font-weight: bold;">Output:</span></pre>
<pre><span style="font-weight: bold;">1</span></pre>
<pre><span style="font-weight: bold;"><div style="background-image: initial; background-attachment: initial; background-origin: initial; background-clip: initial; background-color: white; border-image: initial; padding-right: 20px; padding-left: 20px; padding-top: 5px; padding-bottom: 10px; margin-bottom: 15px; font-family: Arial, Helvetica, sans-serif; font-size: 14px; text-align: -webkit-left; border: 1px solid black;"><span style="font-family: monospace;"><span style="white-space: pre-wrap;">Output explanation:</span></span></div><div style="background-image: initial; background-attachment: initial; background-origin: initial; background-clip: initial; background-color: white; border-image: initial; padding-right: 20px; padding-left: 20px; padding-top: 5px; padding-bottom: 10px; margin-bottom: 15px; font-family: Arial, Helvetica, sans-serif; font-size: 14px; text-align: -webkit-left; border: 1px solid black;"><span id="probtext-text" style="font-family: monospace !important; white-space: pre-wrap;">Removing either post 1 or post 2 will allow Bessie to escape. </span></div><br></span></pre>