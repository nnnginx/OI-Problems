<p>&nbsp;</p>
<p>During recession, Amjad needs to queue for SembakoPlus. Sembako, as we all know, stands for ¡°Sembilan Bahan Pokok¡± which consists of 9 kinds of item: Rice, Sugar, Cooking-oil, Meat, Egg, Milk, Corn, Kerosene and Iodized Salt. SembakoPlus consists of Sembako and one more item: Indomie! Amjad¡¯s favorite of all time!! (therefore, no wonder why he could stand for this long queue).</p>
<p>Each person in the queue is allowed to pick only one item. No need to ask, Amjad wants only Indomie. Unfortunately, they are running out of SembakoPlus stock and currently there are three kinds of item left: Rice, Sugar and Indomie. As he could see from afar, he is quite sure that Rice and Sugar will be enough for everybody.</p>
<p>Given the number of remaining Indomie and the number of people queuing in front of Amjad, your task is to count the probability that he will get his Indomie. Amjad can¡¯t do programming right now as he is very nervous so he can¡¯t think logically. He needs your help!</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>There will be multiple test cases for this problem. Each test case contains two integers N (1 ¡Ü N ¡Ü 50) and S (0 ¡Ü S ¡Ü 50), where N is the number of people queuing in front of Amjad and S is the remaining number of Indomie.</p>
<div><strong>Output</strong></div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>For each case, print in a single line the probability in percentage that he will get his Indomie with 5 digits precision (he¡¯s being paranoid)</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 1
3 2
4 0
4 1
10 10
14 9
30 14


<strong>Output:</strong>
50.00000
76.92308
0.00000
33.33333
99.99831
98.65515
95.16071
</pre>
<div>
<div style="text-align: left;">Explanation for 1st sample test case:</div>
<div style="text-align: left;">There are two peoples queuing in front of Amjad, so those two peoples could pick of the</div>
<div style="text-align: left;">following combination {1st people, 2nd people}:</div>
<div style="text-align: left;">1. Rice, Rice</div>
<div style="text-align: left;">2. Rice, Sugar</div>
<div style="text-align: left;">3. Rice, Indomie</div>
<div style="text-align: left;">4. Sugar, Rice</div>
<div style="text-align: left;">5. Sugar, Sugar</div>
<div style="text-align: left;">6. Sugar, Indomie</div>
<div style="text-align: left;">7. Indomie, Rice</div>
<div style="text-align: left;">8. Indomie, Sugar</div>
<div style="text-align: left;">Since there is only one Indomie left, there are only 4 out of 8 combinations that ensure Amjad&nbsp;to get his Indomie (1, 2, 4 and 5), hence the probability is 4/8 = 50%.</div>
</div>