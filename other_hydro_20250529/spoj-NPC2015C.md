<p>Doto is a famous game. In that game, each player controls N heroes where each heroes has an infinite number of skills. These skills can be used to empower other heroes. Eefun is currently playing with his N heroes, numbered from 1 to N.</p>
<p>The main objective of this game is to defeat the enemies with these heroes. However, Eefun always lose the game, so now Eefun only try to make his heroes powerful.</p>
<p>Based on Eefun's logic, there are M requirements to make all of his heroes powerful. Each requirement needs a hero A and a hero B. Hero A must use his/her skill to hero B to make B more powerful. Moreover, if hero B and C needs skill from hero A, hero A can use his/her skill to hero B. Then, hero B skills will be empowered with skills from hero A. Therefore, he can use his skill to hero C. In this scenario, the number of skills activated is 2, where A doesn't get any skills, B get skill from hero A, and C get skill from both hero A and B.</p>
<p>The skill is continuous, so if A give his skill to B, B give his skill to C, and C give his skill to A, then every hero get every other heroes skills</p>
<p>Now Eefun is curious, how many skills must be activated to complete all his requirements&nbsp;</p>
<h3>Input</h3>
<p>First line consists of 2 integers, N and M which denotes number of heroes and requirements.<br>Next M skills each contains 2 integers, A and B, which means hero B will be powerful if he get skills from hero A.&nbsp;</p>
<h3>Output</h3>
<p>Output an integer, the minimum number of skills which must be activated to complete all the requirements</p>
<h3>Example</h3>
<pre><strong>Input 1:</strong>
3 4
1 2
2 3
3 1
2 1

<strong>Output 1:</strong>
3

<strong>Input 2:</strong>
5 5
1 5
3 4
4 3
2 5
1 3

<strong>Output 2:</strong>
5
</pre>
<div style="border: 1px solid #ADC; background-color: #0cc; padding: 5px; margin-bottom: 10px;">
<h3>Explanation</h3>
<ul>
<li>For the first case, hero 1 can give his skill to hero 2, hero 2 can give his skill to hero 3, and hero 3 can give his skill to hero 1.</li>
<li>For the second case, one of the configuration is like in the picture below :<br><img src="file://e1kF8SOw.png" alt="" width="640" height="371">&nbsp;</li>
</ul>
</div>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>A ¡Ù B</li>
<li>1 ¡Ü A,B ¡Ü N</li>
<li>1 ¡Ü N ¡Ü 100.000</li>
<li>1 ¡Ü M ¡Ü 100.000</li>
</ul>
</div>