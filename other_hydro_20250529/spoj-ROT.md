<p>&nbsp;</p>
<p>In the future there is an agency that works on rescuing people from the “bad guys”, those guys are a super secret evil agency that is on a super secret bunker that everybody knows, especially the agency we mentioned before. This agency (the good one) has a very particular thing, they can do time travel either to the future or to the past and they can do it how many times they want, but only one minute to the future or one minute to the past,or even stay in the present, it is impossible to go for example three minutes to the future or two minutes to the past; our agency wants to rescue only one hostage since the “bad guys” are really dumb and they can kidnap only one person and keep it hidden (it is dumb because the bunker is huge), now here is the deal, the agency has contracted us to do a program that tells the minimum number of time steps the agent of our agency should make to save the hostage (I am so lazy that you will do it all by yourself). It is important to know that at some point after certain amount of time the hostage will be killed so we don´t want to go over that time, never! And also we don´t want to get back on a time where the hostage isn´t in the bunker yet so remember that!, he can take a step into any adjacent direction but not in diagonals, and it is no meaning into wait on a position because the agent can use time as he wants.</p>
<p>&nbsp;</p>
<p>‘X’-&gt; represents the place where the agent starts, it is guaranteed that the agent starts at the time 1</p>
<p>‘#’-&gt; represents a wall</p>
<p>‘s’-&gt;represents a free space</p>
<p>‘!’-&gt; represents a “bad guy”</p>
<p>‘O’-&gt;represents our objective</p>
<h3>Input</h3>
<p>The first line of input is T the number of test cases, there will be several test cases T&lt;=10. Next line of input contains C,R,Time, which are Columns&lt;=15, Rows&lt;=15 and of course the Time&lt;=10 (Right after that maximum time the hostage will be killed and before time 1 there will be no hostage to save so is useless to go there) Time is measured in minutes, after that, Time lines will follow with a matrix of RxC Representing the actual position of guards and new free spaces after time traveling (Obviously walls will not move, and neither does the hostage because he is tide up)</p>
<h3>Output</h3>
<p>Just output the minimum number of time steps that takes to our agent to get to the hostage, if it is impossible to get to the Hostage then should output: “Hostage is death, destroy the bunker”</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>3 3 1
</p><p>sss<br>ssX
Oss</p>3 3 3
Xss&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
#s!
s!O
sss
#!s
!sO
ss!
#s!
ssO<br><br><strong>Output:</strong>
3<br>4 <br></pre>