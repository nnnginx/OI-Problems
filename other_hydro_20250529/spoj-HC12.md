<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">John is playing a game with his friends. The game's rules are as follows: There is deck of&nbsp;<strong>N</strong>&nbsp;cards from which each person is dealt a hand of&nbsp;<strong>K</strong>&nbsp;cards. Each card has an integer value representing its strength. A hand's strength is determined by the value of the highest card in the hand. The person with the strongest hand wins the round. Bets are placed before each player reveals the strength of their hand.</span></p>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">John needs your help to decide when to bet. He decides he wants to bet when the strength of his hand is higher than the average hand strength. Hence John wants to calculate the average strength of ALL possible sets of hands. John is very good at division, but he needs your help in calculating the sum of the strengths of all possible hands.</span></p>
<h2 style="color: #333333; margin: 0px; padding: 0px; line-height: 16px;"><span style="font-size: small;">Problem</span></h2>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">You are given an array&nbsp;<strong>a</strong>&nbsp;with&nbsp;<strong>N �� 10 000</strong>&nbsp;different integer numbers and a number,&nbsp;<strong>K</strong>, where&nbsp;<strong>1 �� K �� N</strong>. For all possible subsets of&nbsp;<strong>a</strong>&nbsp;of size&nbsp;<strong>K</strong>&nbsp;find the sum of their maximal elements modulo&nbsp;<strong>1 000 000 007</strong>.</span></p>
<h2 style="color: #333333; margin: 0px; padding: 0px; line-height: 16px;"><span style="font-size: small;">Input</span></h2>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">The first line contains the number of test cases&nbsp;<strong>T</strong>, where&nbsp;<strong>1 �� T �� 25</strong></span></p>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">Each case begins with a line containing integers&nbsp;<strong>N</strong>&nbsp;and&nbsp;<strong>K</strong>. The next line contains&nbsp;<strong>N</strong>&nbsp;space-separated numbers&nbsp;<strong>0 �� a [i] �� 2 000 000 000</strong>, which describe the array&nbsp;<strong>a</strong>.</span></p>
<h2 style="color: #333333; margin: 0px; padding: 0px; line-height: 16px;"><span style="font-size: small;">Output</span></h2>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">For test case&nbsp;<strong>i</strong>, numbered from&nbsp;<strong>1</strong>&nbsp;to&nbsp;<strong>T</strong>, output "Case #i: ", followed by a single integer, the sum of maximal elements for all subsets of size&nbsp;<strong>K</strong>&nbsp;modulo 1 000 000 007.</span></p>
<p style="margin: 1em 0px;"><span style="line-height: 16px;"><span style="font-size: small;"> </span></span></p>
<p style="margin: 1em 0px;"><strong>Example input</strong></p>
<p style="margin: 1em 0px;">5</p>
<p style="margin: 1em 0px;">4 3</p>
<p style="margin: 1em 0px;">3 6 2 8&nbsp;</p>
<p style="margin: 1em 0px;">5 2</p>
<p style="margin: 1em 0px;">10 20 30 40 50&nbsp;</p>
<p style="margin: 1em 0px;">6 4</p>
<p style="margin: 1em 0px;">0 1 2 3 5 8&nbsp;</p>
<p style="margin: 1em 0px;">2 2</p>
<p style="margin: 1em 0px;">1069 1122&nbsp;</p>
<p style="margin: 1em 0px;">10 5</p>
<p style="margin: 1em 0px;">10386 10257 10432 10087 10381 10035 10167 10206 10347 10088&nbsp;</p>
<p style="margin: 1em 0px;"><strong>Example output</strong></p>
<p style="margin: 1em 0px;">Case #1: 30</p>
<p style="margin: 1em 0px;">Case #2: 400</p>
<p style="margin: 1em 0px;">Case #3: 103</p>
<p style="margin: 1em 0px;">Case #4: 1122</p>
<p style="margin: 1em 0px;">Case #5: 2621483</p>
<p>&nbsp;</p>
<p style="margin: 1em 0px; color: #333333; line-height: 16px;"><span style="font-size: small;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Example input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">4 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">3 6 2 8&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">5 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 20 30 40 50&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">6 4</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">0 1 2 3 5 8&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1069 1122&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10386 10257 10432 10087 10381 10035 10167 10206 10347 10088&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Example output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #1: 30</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #2: 400</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #3: 103</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #4: 1122</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #5: 2621483Example input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">4 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">3 6 2 8&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">5 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 20 30 40 50&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">6 4</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">0 1 2 3 5 8&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1069 1122&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10386 10257 10432 10087 10381 10035 10167 10206 10347 10088&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><br></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;"><br></span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Example output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #1: 30</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #2: 400</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #3: 103</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #4: 1122</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Case #5: 2621483</span></div>
<p>&nbsp;</p>