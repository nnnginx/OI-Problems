<p>Trouble has befallen the ninja world (again!). As always, our hero Naruto has taken the responsibility to defend everyone from the evil forces. His signature attack is the cloning jutsu (i.e. cloning technique) in which he produces one clone of himself in one second. Each clone of Naruto can also perform the cloning technique.<br><br>Naruto arrives alone at the battlefield at t=1 second. At each time step , t= 1,2,3,¡­.,n second , some of the Narutos will leave to start fighting the enemy and the rest will stay back and perform the cloning jutsu again. If a clone&nbsp; has left to fight the enemy he cannot come back to perform the jutsu. Also at t=n seconds all Narutos will go to fight with the enemy, i. e. no more cloning will take place on and after n seconds. Naruto is a very dedicated ninja so he won¡¯t allow any of his clone to stay out of the fight.<br>The commander of the ninja forces observes Naruto¡¯s actions. He notes down the number of clones that went to fight the enemy at each time step( from t=1 second till t=n second).&nbsp; However he is old and doubts if his observations are correct. He hires you, a ninja with sharp analytical skills, to check if his observations can be&nbsp; valid or not.<br><br><strong>INPUT:</strong><br><br>The first line of the input contains t the number of test cases. The first line of each test case contains n, the time when all Naruto clones go to fight. In the second line of each test case there are n space separated integers that tell how many Naruto clones went to fight at successive seconds, starting from t = 1 second till t = n seconds;<br><br><strong>OUTPUT:</strong><br><br>For each test case output either ¡°Yes¡± or ¡°No¡± (without quotes) in a single line. ¡°Yes¡± if the commander¡¯s observations were correct and ¡°No¡± if they were wrong;<br><br><strong>CONSTRAINTS:</strong><br><br>1&lt;= T &lt;= 20<br><br>1&lt;= n &lt;=10^6<br><br>Each of the n integers will be less than or equal to 2 ^ 30</p>
<p><strong>SAMPLE TEST CASES:</strong></p>
<p><strong><br>INPUT:</strong></p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">0 0 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">0 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 218px; width: 1px; height: 1px; overflow: hidden;">0 1 2</div>
<p>3</p>
<p>3</p>
<p>0 0 4</p>
<p>2</p>
<p>0 5</p>
<p>3</p>
<p>0 1 2</p>
<p><strong>OUTPUT:</strong></p>
<p>Yes</p>
<p>No</p>
<p>Yes</p>
<p><br><br><strong>EXPLANATION:</strong><br><br>For the sample test case 2 :<br><br>2<br><br>0 5<br><br>At t = 1 second, Naruto population is 1. According to the commander¡¯s observations no Naruto leaves to fight at t=1 ( and all will perform the cloning jutsu), so the population will become 1 X 2= 2. He observed that at t=2 seconds, 5 narutos went to fight. This is not possible as at t=2 seconds the Naruto population is only 2. Therefore, the commander¡¯s observations are incorrect.</p>
<p>&nbsp;</p>