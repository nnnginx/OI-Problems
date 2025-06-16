<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'We fought far under the living earth, where time is not counted. Ever he clutched me, and ever I hewed him, till at last he fled into dark tunnels. Ever up now we went, until we came to the Endless Stair. Out he sprang, and even as I came behind, he burst into new flame. Those that looked up from afar thought that the mountain was crowned with storm. Thunder they heard, and lightning, they said, smote upon Celebdil, and leaped back broken into tongues of fire.' - Gandalf, describing his fight against the Balrog.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Although Gandalf would not go into the details of his battle, they can be summarized into the following simplified form: both Gandalf and the Balrog have a set of N attacks they can use (spells, swords, brute-force strength etc.). These attacks are numbered from 1 to N in increasing order of Power. When each has chosen an attack, in general, the one with the higher power wins. However, there are a few ("M") anomalous pairs of attacks, in which the lesser-powered attack wins.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Initially, Gandalf picks an attack. Then the Balrog counters it with one of the remaining attacks. If the Balrog's counter does not defeat Gandalf's, then we say Gandalf receives a score of 2. If however it does, then Gandalf has exactly one more opportunity to pick an attack that will defeat the Balrog's. If he manages to defeat him now, his score will be 1, whereas if he is still unable to defeat him, his score will be 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to determine, given N and the M anomalous pairs of attacks, what will be Gandalf's score, given that both play optimally. Further, in case Gandalf gets a score of 2, you must also determine which attack he could have chosen as his first choice.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note 1: The Balrog can choose only one attack, whereas Gandalf can choose upto two.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note 2: The relation A defeats B is not transitive within the attacks. For example, attack A can defeat attack B, attack B can defeat attack C, and attack C can defeat attack A.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note 3: Between any two attacks A and B, either attack A defeats attack B or attack B defeats attack A.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line will consist of the integer T, the number of test-cases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case begins with a single line containing two integers N and M.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This is followed by M lines consisting of 2 integers each x and y, denoting that x and y are an anomalous pair.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each test-case, output a single line either</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 A, if Gandalf can defeat any attack the Balrog chooses if he picks attack A,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1, if Gandalf can choose an attack such that even if the Balrog chooses an attack to defeat him, he can choose an attack to defeat the Balrog's chosen card,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0, if none of the above two options are possible for all possible choices of Gandalf's attack(s).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Between successive test cases, there should not be any blank lines in the output.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 15</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 &lt;= N &lt;= 1,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= M &lt;= min(N(N-1)/2, 300,000)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= x &lt; y &lt;= N for all the anomalous pairs (x,y)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The sum of M over all test-cases will not exceed 300,000.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Time Limit: 4s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Memory Limit: 64MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 3&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first case, attack 3 can beat both attacks 1 and 2. So Gandalf just chooses attack 3.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the second case, attack 1 beats 3 which beats 2 which beats 1. No matter which attack Gandalf chooses, the Balrog can pick the one which defeats his, but then he can pick the remaining attack and defeat the Balrog's.</div>
<p>'We fought far under the living earth, where time is not counted. Ever he clutched me, and ever I hewed him, till at last he fled into dark tunnels. Ever up now we went, until we came to the Endless Stair. Out he sprang, and even as I came behind, he burst into new flame. Those that looked up from afar thought that the mountain was crowned with storm. Thunder they heard, and lightning, they said, smote upon Celebdil, and leaped back broken into tongues of fire.' - Gandalf, describing his fight against the Balrog.</p>
<p>&nbsp;</p>
<p>Although Gandalf would not go into the details of his battle, they can be summarized into the following simplified form: both Gandalf and the Balrog have a set of N attacks they can use (spells, swords, brute-force strength etc.). These attacks are numbered from 1 to N in increasing order of Power. When each has chosen an attack, in general, the one with the higher power wins. However, there are a few ("M") anomalous pairs of attacks, in which the lesser-powered attack wins.</p>
<p>&nbsp;</p>
<p>Initially, Gandalf picks an attack. Then the Balrog counters it with one of the remaining attacks. If the Balrog's counter does not defeat Gandalf's, then we say Gandalf receives a score of 2. If however it does, then Gandalf has exactly one more opportunity to pick an attack that will defeat the Balrog's. If he manages to defeat him now, his score will be 1, whereas if he is still unable to defeat him, his score will be 0.</p>
<p>&nbsp;</p>
<p>Your task is to determine, given N and the M anomalous pairs of attacks, what will be Gandalf's score, given that both play optimally. Further, in case Gandalf gets a score of 2, you must also determine which attack he could have chosen as his first choice.</p>
<p>&nbsp;</p>
<p>Note 1: The Balrog can choose only one attack, whereas Gandalf can choose upto two.</p>
<p>Note 2: The relation A defeats B is not transitive within the attacks. For example, attack A can defeat attack B, attack B can defeat attack C, and attack C can defeat attack A.</p>
<p>Note 3: Between any two attacks A and B, either attack A defeats attack B or attack B defeats attack A.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line will consist of the integer T, the number of test-cases.</p>
<p>Each test case begins with a single line containing two integers N and M.</p>
<p>This is followed by M lines consisting of 2 integers each x and y, denoting that x and y are an anomalous pair.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each test-case, output a single line either</p>
<p>2 A, if Gandalf can defeat any attack the Balrog chooses if he picks attack A,</p>
<p>1, if Gandalf can choose an attack such that even if the Balrog chooses an attack to defeat him, he can choose an attack to defeat the Balrog's chosen card,</p>
<p>0, if none of the above two options are possible for all possible choices of Gandalf's attack(s).</p>
<p>Between successive test cases, there should not be any blank lines in the output.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 15</p>
<p>3 &lt;= N &lt;= 1,000,000</p>
<p>0 &lt;= M &lt;= min(N(N-1)/2, 300,000)</p>
<p>1 &lt;= x &lt; y &lt;= N for all the anomalous pairs (x,y)</p>
<p>The sum of M over all test-cases will not exceed 300,000.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3 0</p>
<p>3 1</p>
<p>1 3&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2 3</p>
<p>1</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>In the first case, attack 3 can beat both attacks 1 and 2. So Gandalf just chooses attack 3.</p>
<p>In the second case, attack 1 beats 3 which beats 2 which beats 1. No matter which attack Gandalf chooses, the Balrog can pick the one which defeats his, but then he can pick the remaining attack and defeat the Balrog's.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>