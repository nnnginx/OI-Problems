<p>
You have a revolver gun with a cylinder that has n chambers. Chambers are located in a circle on a&nbsp;cylinder. Each chamber can be empty or can contain a round. One chamber is aligned with the gun's&nbsp;barrel. When trigger of the gun is pulled, the gun's cylinder rotates, aligning the next chamber with the&nbsp;barrel, hammer strikes the round, making a shot by firing a bullet through the barrel. If the chamber is&nbsp;empty when the hammer strikes it, then there is no shot but just a "click".
</p>

<p>
You have found a use for this gun. You are playing Russian Roulette with your friend. Your friend loads&nbsp;rounds into some chambers, randomly rotates the cylinder, aligning a random chamber with a gun's&nbsp;barrel, puts the gun to his head and pulls the trigger. You hear "click" and nothing else - the chamber&nbsp;was empty and the gun did not shoot.
</p>

<p>
Now it is your turn to put the gun to your head and pull the trigger. You have a choice. You can either&nbsp;pull the trigger right away or you can randomly rotate the gun's cylinder and then pull the trigger. What&nbsp;should you choose to maximize the chances of your survival?
</p>

<h3>Input</h3>
<p>
The input first line contains a single line with a string of n digits "<tt>0</tt>" and "<tt>1</tt>" (2 &lt;= n &lt;= 100). This line of&nbsp;digits represents the pattern of rounds that were loaded into the gun's chambers. "<tt>0</tt>" represent an empty&nbsp;chamber, "<tt>1</tt>" represent a loaded one. In this representation, when cylinder rotates before a shot, the&nbsp;next chamber to the right gets aligned with the barrel for a shot. Since the chambers are actually located&nbsp;on a circle, the first chamber in this string follows the last one. There is at least one "0" in this string.
</p>

<h3>Output</h3>
<p>Write to the output single one of the following words (without quotes): </p>
<ul>
  <li>"<tt>SHOOT</tt>" - if pulling the trigger right away makes you less likely to be actually shot in the head&nbsp;with the bullet (more likely that the chamber will be empty). </li>
  <li>"<tt>ROTATE</tt>" - if randomly rotating the cylinder before pulling the trigger makes you less likely to be&nbsp;actually shot in the head with the bullet (more likely that the chamber will be empty). </li>
  <li>"<tt>EQUAL</tt>" - if both of the above choices are equal in terms of probability of being shot. </li>
</ul>

<h3>Example</h3>
<pre><strong>Input:</strong>
0011

<strong>Output:</strong>
EQUAL</pre>

<pre><strong>Input:</strong>
0111

<strong>Output:</strong>
ROTATE</pre>

<pre><strong>Input:</strong>
000111
  
<strong>Output:</strong>
SHOOT</pre>