<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Middle Earth&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Barbarians in Middle-Earth consider pillaging villages a sport and they are quite fond of it. Hussain the greatest barbarian in the world arrived to Gondor, and wants to prove himself by pillaging as many villages as he can.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are N villages in Gondor that Hussain can pillage in any order he likes, but to pillage village i he has to spend Ai golden coins from his personal bank account on weapons and armor to successfully pillage that village otherwise he will die in the attack, but if his attack is successful he will loot Bi golden coins and add it to his personal bank account.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Hussain starts with C golden coins in his bank account and due to his barbarian code of honor he will keep attacking villages until he either pillages all villages or dies.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Barbarians define a strong village if and only if Ai&gt;Bi, Hussain also knows based on the BEAA (Barbarian Enemy Analysis Algorithm) that in Gondor there will never be more than 15 strong villages.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">And because Hussain is a proud barbarian and wants to bring honor to his tribe he asked you to determine the maximum number of villages that he can successfully pillage.</div>
<p>Barbarians in Middle-Earth consider pillaging villages a sport and they are quite fond of it. Hussain the greatest barbarian in the world arrived to Gondor, and wants to prove himself by pillaging as many villages as he can.&nbsp;</p>
<p>There are N villages in Gondor that Hussain can pillage in any order he likes, but to pillage village i he has to spend Ai golden coins from his personal bank account on weapons and armor to successfully pillage that village otherwise he will die in the attack, but if his attack is successful he will loot Bi golden coins and add it to his personal bank account.&nbsp;</p>
<p>Hussain starts with C golden coins in his bank account and due to his barbarian code of honor he will keep attacking villages until he either pillages all villages or dies.&nbsp;</p>
<p>Barbarians define a strong village if and only if Ai&gt;Bi, Hussain also knows based on the BEAA (Barbarian Enemy Analysis Algorithm) that in Gondor there will never be more than 15 strong villages <strong>that could be attacked at any time </strong>(That means if there is a village that could never be attacked the algorithm will simply ignore it).&nbsp;</p>
<p>And because Hussain is a proud barbarian and wants to bring honor to his tribe he asked you to determine the maximum number of villages that he can successfully pillage.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of input contains T (the number of test cases).&nbsp;</p>
<p>The first line of each test case contains 2 integers separated by spaces (1 ¡Ü n ¡Ü 10^5) and (1¡Ü C ¡Ü 10^9).&nbsp;</p>
<p>The following N lines contain 2 integers separated by spaces (1 ¡Ü Ai, Bi ¡Ü 10^9).&nbsp;</p>
<h3>Output</h3>
<p>The answer to each test case separated by a new line.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 
4 2 
2 10 
1 0 
10 23 
54 44

<strong>Output:</strong>
3 
</pre>