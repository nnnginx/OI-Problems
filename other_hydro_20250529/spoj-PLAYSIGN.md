<p>You and Dope are visiting DAKSH. Suddenly Dope found some balls having some mass  on it and all balls are white in color. They found an interesting thing of the balls that they can  change color to either red or green on clicking the switch on it.Dope is in a funny  mood and wants to play a game with you.  He tells you that each player will switch the balls to either red or green color alternatively and  only white ball can be chosen to change the color.After changing the color of all balls you need  to pay an amount equal to the absolute difference between mass of the red balls and green balls.  Dopen would try to maximize the pay and obviously you want to give him as less as possible.  Dope invites you to play first. If you and Dope  play optimally, what is the amount you  have to pay to Dope?</p>
<h3>Input</h3>
<p>T number of test cases. Each case consists of two lines. first line N number of white balls. Next line contains a b c use to generate N mass using<br>mass = (a*i+b)%c; for 1&lt;=i&lt;=N<br></p>
<h3>Output</h3>
<p>single line for each case the amount you need to pay</p>
<p>limit:<br>1&lt;=T&lt;1000<br>1&lt;=N&lt;10000</p>
<p>1&lt;=a,c&lt;1000<br>0&lt;=b&lt;1000</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>3<br>1 0 10<br>4<br>2 1 10<br><strong>Output:</strong>
<br>2<br>10<br><br>explanation:<br>case1: 3 mass = 1 2 3; output = 2<br>case2: 4 mass=3 5 7 9;output=10 </pre>