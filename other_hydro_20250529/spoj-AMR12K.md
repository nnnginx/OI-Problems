<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'I think that the enemy brought his own enemy with him,' answered Aragorn. 'These are Northern Orcs from far away. Among the slain are none of the great Orcs with the strange badges. There was a quarrel, I guess: it is no uncommon thing with these foul folk. Maybe there was some dispute about the road.' - Aragorn describing the nature of Orcs.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Indeed, everyone knows that the Orcs are treacherous creatures who look for their own satisfaction and more often than not disregard the rules. The only way to keep them in line, is by maintaining the chain of command over a strict hierarchy among the ranks, wherein each Orc is responsible to his immediate superior all the way up to the army's head.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Further, the powers that be, have decided to have regular checks of their army's loyalties, just in case some Orc has been killed and all his juniors end up turning rogue!</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are N orcs, numbered 1 to N, wherein the lead orc is numbered 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Step 1. Randomly choose a fixed order in which to test Orcs' loyalties.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Step 2. Going in this order, you make a "roll-call" to check if the current Orc is alive or not.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Step 3. If the current Orc is dead, then he is marked as "deleted".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">With this information, it is possible to tell which all Orcs will be loyal, and which won't be. However, cunning Master Wormtongue suggests the following optimization:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In step 2, if any of the considered Orc's superiors (not necessarily immediate superior) is marked as deleted, then the roll-call is not made.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now, given this algorithm and the hierarchy of the army, along with which Orcs are dead, what is the expected number of roll-calls (taken over all possible orderings in "Step 1") that you save by performing this optimization?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains T, the number of test cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line of each test case contains N, the number of orcs in the army. The next N-1 lines contain two space-separated integers u v, denoting that u is the immediate superior of v or vice-versa. The head of the army is the orc labelled 1. The next line contains m, the number of dead orcs. The next line contains m space separated integers, which are the labels of the dead orcs.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output one real number for each test case containing the expected number of roll-calls that you save. The results should be accurate within an error range of 10^-6.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= N &lt;= 100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= u, v &lt;= N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">u != v</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The given set of u-v pairs form a valid chain of command. That means every Orc, except the Orc labeeled 1, has exactly one immediate superior.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0.5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the first test case, the Orc labelled 1 is dead. The two possible orderings are [1, 2] and [2, 1]. With the optimization, for the order [1, 2], we save the roll-call to 2. So, the total number of roll-calls without the optimization is 4, and with the optimization is 3. Expected number of roll-calls is therefore, (4 - 3) / 2 = 0.5 .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the second test case, the Orc labeled 2 is dead. Since he does not have any sub-ordinates, the optimization does not have any effect.</div>
<p>&nbsp;</p>
<p>'I think that the enemy brought his own enemy with him,' answered Aragorn. 'These are Northern Orcs from far away. Among the slain are none of the great Orcs with the strange badges. There was a quarrel, I guess: it is no uncommon thing with these foul folk. Maybe there was some dispute about the road.' - Aragorn describing the nature of Orcs.</p>
<p>&nbsp;</p>
<p>Indeed, everyone knows that the Orcs are treacherous creatures who look for their own satisfaction and more often than not disregard the rules. The only way to keep them in line, is by maintaining the chain of command over a strict hierarchy among the ranks, wherein each Orc is responsible to his immediate superior all the way up to the army's head.</p>
<p>&nbsp;</p>
<p>Further, the powers that be, have decided to have regular checks of their army's loyalties, just in case some Orc has been killed and all his juniors end up turning rogue!</p>
<p>&nbsp;</p>
<p>There are N orcs, numbered 1 to N, wherein the lead orc is numbered 1.</p>
<p>Step 1. Randomly choose a fixed order in which to test Orcs' loyalties.</p>
<p>Step 2. Going in this order, you make a "roll-call" to check if the current Orc is alive or not.</p>
<p>Step 3. If the current Orc is dead, then he is marked as "deleted".</p>
<p>&nbsp;</p>
<p>With this information, it is possible to tell which all Orcs will be loyal, and which won't be. However, cunning Master Wormtongue suggests the following optimization:</p>
<p>In step 2, if any of the considered Orc's superiors (not necessarily immediate superior) is marked as deleted, then the roll-call is not made.</p>
<p>&nbsp;</p>
<p>Now, given this algorithm and the hierarchy of the army, along with which Orcs are dead, what is the expected number of roll-calls (taken over all possible orderings in "Step 1") that you save by performing this optimization?</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains T, the number of test cases.</p>
<p>The first line of each test case contains N, the number of orcs in the army. The next N-1 lines contain two space-separated integers u v, denoting that u is the immediate superior of v or vice-versa. The head of the army is the orc labelled 1. The next line contains m, the number of dead orcs. The next line contains m space separated integers, which are the labels of the dead orcs.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output one real number for each test case containing the expected number of roll-calls that you save. The results should be accurate within an error range of 10^-6.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 5</p>
<p>1 &lt;= N &lt;= 100,000</p>
<p>1 &lt;= u, v &lt;= N</p>
<p>u != v</p>
<p>The given set of u-v pairs form a valid chain of command. That means every Orc, except the Orc labeeled 1, has exactly one immediate superior.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>2</p>
<p>1 2</p>
<p>1</p>
<p>1</p>
<p>2</p>
<p>1 2</p>
<p>1</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>0.5</p>
<p>0</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>For the first test case, the Orc labelled 1 is dead. The two possible orderings are [1, 2] and [2, 1]. With the optimization, for the order [1, 2], we save the roll-call to 2. So, the total number of roll-calls without the optimization is 4, and with the optimization is 3. Expected number of roll-calls is therefore, (4 - 3) / 2 = 0.5 .</p>
<p>For the second test case, the Orc labeled 2 is dead. Since he does not have any sub-ordinates, the optimization does not have any effect.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>