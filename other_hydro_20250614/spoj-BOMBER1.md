<pre><br>You are requested to donate your two cents to help us build a better nation: https://donate.aamaadmiparty.org/  </pre>
<p>&nbsp;</p>
<p>Jay and Nemo are galactic wanderers. While travelling around in Bomber Nebula, they decided to spend some time  in the famous Bingeling Empire. To manage their expenses, they took up an internship under Dr.Ein, the scientist assisting the Bomberman.</p>
<p>Unfortunately at the same time, Fiendish Bombers penetrated the defenses of the planet Bomber and have swarmed the entire empire. Consider the empire as<strong> NxNxN </strong>maze with each cell occupied by the enemy. You can also view it as a huge cube with side <strong>N</strong>.</p>
<p>The task of Jay and Nemo is now to guide the Bomberman to plant the bombs and destroy enemies. Because one of Dr. Ein's new invention, the Fire ability of the Bomberman��s bomb is infinite. That is, if it explodes at <strong>(x,y,z)</strong> it will destroy enemies in all the cells <strong>(*,y,z)</strong> ,<strong> (x,*,z) </strong>and <strong>(x,y,*)</strong>. Since most of the resources of the empire are captured, they are left with only <strong>M</strong> bombs. Although being good computer scientists, they are exceptionally poor at visualising things in 3 dimensions. So they ask you, &lt;insert your name here&gt; the greatest programmer ever to roam on Earth: Is is possible to defeat the invaders?</p>
<h3>Input</h3>
<p>The first line contains <strong>T</strong>, the number of test cases. Each of the next <strong>T</strong> lines contains 2 space separated integers <strong>N</strong> and <strong>M</strong>, denoting the size of the maze and the count of available bombs respectively.</p>
<h3>Output</h3>
<p>"<strong>POSSIBLE</strong>" or "<strong>IMPOSSIBLE</strong>"&nbsp; depending upon each test case.</p>
<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 10^6</p>
<p>1 &lt;= N &lt;= 10^7</p>
<p>0 &lt;= M &lt;= 10^16</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>1 0<br>1 1<br>1 2<br>2 1<br><br><br><strong>Output:</strong>
IMPOSSIBLE<br>POSSIBLE<br>POSSIBLE<br>IMPOSSIBLE<br><br>
Warning: Large I/O. Tested for most languages, but let me know if you are getting TLE.<br></pre>