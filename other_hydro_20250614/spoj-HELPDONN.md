<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">PROBLEM CODE:Enigma Treasure Hunt</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;"><span style="white-space: pre;"> </span>KaushikRamDonn went to Enigma and registered for&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Treasure Hunt.Following are the rules for Enigma Treasure hunt ,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule 1: Donn has to go from 1st stage to nth stage in a sequential order ( only after completing stage 1 ,he can go to stage 2,then to stage 3).&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">and collect treasures in a bag</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule2: Donn will be given only k bags at the time of registration</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule3: There are bags capable of holding all possible weights and is infinite in number. Donn is free to choose any bags capable of holding any weight (but all the k bags should be capable of holding the same weight)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Pandian,the organiser will give the bag ,Euler asked.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule4: once the game is started ,Donn cant exchange his bag .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule5: While going through different stages,if Donn couldnt accomodate the treasure in a bag ,tie the bag and give it to Pandian.(this bag cant be used any more.Then start collecting the treasures in a new bag.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Rule6: The cost of the bag is directly proportional to the weight it can hold ,so try to reduce the cost.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Fortunatley ,Donn knows the weights of the treasure in each stage ,Help Donn Choose his bag (maximum bag size needed) .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Example:&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Consider there are 3 stages(n= 3) in the Hunt.the weight of the treasures in each of these stages (which is known to donn before the hunt starts)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">are 1,2 and 3. Donn is &nbsp;allowed to get 2 bags(k= 2) in this example</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">n = 3, k= 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">stages = {1,2,3}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Donn could accomplish his target if each of his bag can accomodate 3 kg or 5 kg.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Explanation :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">if the wieght of the bag is 3 - Stage1 weight + stage2 weight = 1+2=3 &lt;=3 in one bag ,stage 3 weight= 3&lt;=3 &nbsp;in another bag.thus they fit in the bags</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">if the wieght of the bag is 5 - Stage1 weight = 1&lt;=5 in one bag,stage2 + stage 3 weight= 2+3 =5 &lt;=5 in another bag.thus they fit in the bags</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">but consider a bag size of 2 :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">1 + 2&gt; 2 so put stage1 treasure alone in 1st bag</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">2 + 3 &gt;2 so put stage2 treasure alone in 2st bag</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">now we need one more bag to put in the 3rd treasure.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">This is not possible so u cant choose a bag of size 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">bag of size &gt;=3 can be used&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Donn is intelligent and so he wants to pay the minimum cost so Donn will purchase a bag of size 3.Help Donn solve his problem .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">0&lt; T &lt;=100 ,no of test cases&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Each test case contains</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">0&lt;N&lt;=1000,no of stages and then a space followed by</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">0&lt;k&lt;=1000, no of bags allowed</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">the next N lines contains the weights of the treasures in each stage</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">output a single line containing the minimum size of the bag needed.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Example<span style="white-space: pre;"> </span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">output :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 29px; width: 1px; height: 1px; overflow: hidden;">3&nbsp;</div>
<p>&nbsp;</p>
<p>PROBLEM CODE:Enigma Treasure Hunt</p>
<p><span style="white-space:pre"> </span>KaushikRamDonn went to Enigma and registered for&nbsp;</p>
<p>Treasure Hunt.Following are the rules for Enigma Treasure hunt ,</p>
<p>Rule 1: Donn has to go from 1st stage to nth stage in a sequential order ( only after completing stage 1 ,he can go to stage 2,then to stage 3).&nbsp;</p>
<p>and collect treasures in a bag</p>
<p>Rule2: Donn will be given only k bags at the time of registration</p>
<p>Rule3: There are bags capable of holding all possible weights and is infinite in number. Donn is free to choose any bags capable of holding any weight (but all the k bags should be capable of holding the same weight)</p>
<p>Pandian,the organiser will give the bag to Donn.</p>
<p>Rule4: once the game is started ,Donn cant exchange his bag .</p>
<p>Rule5: While going through different stages,if Donn couldnt accomodate the treasure in a bag ,he will tie the bag and give it to Pandian.(this bag cant be used any more).Then he starts collecting the treasures in a new bag.</p>
<p>Rule6: The cost of the bag is directly proportional to the weight it can hold ,so try to reduce the cost.</p>
<p>Fortunatley ,Donn knows the weights of the treasure in each stage ,Help Donn Choose his bag.</p>
<p>&nbsp;</p>
<p>Example:&nbsp;</p>
<p>&nbsp;</p>
<p>Consider there are 3 stages(n= 3) in the Hunt.the weight of the treasures in each of these stages (which is known to donn before the hunt starts)</p>
<p>are 1,2 and 3. Donn is &nbsp;allowed to get 2 bags(k= 2) in this example</p>
<p>&nbsp;</p>
<p>n = 3, k= 2</p>
<p>stages = {1,2,3}</p>
<p>&nbsp;</p>
<p>Donn could accomplish his target if each of his bag can accomodate 3 kg or 5 kg.</p>
<p>Explanation :</p>
<p>if the wieght of the bag is 3 - Stage1 weight + stage2 weight = 1+2=3 &lt;=3 in one bag ,stage 3 weight= 3&lt;=3 &nbsp;in another bag.thus they fit in the bags</p>
<p>if the wieght of the bag is 5 - Stage1 weight = 1&lt;=5 in one bag,stage2 + stage 3 weight= 2+3 =5 &lt;=5 in another bag.thus they fit in the bags</p>
<p>but consider a bag size of 2 :</p>
<p>1 + 2&gt; 2 so put stage1 treasure alone in 1st bag</p>
<p>2 + 3 &gt;2 so put stage2 treasure alone in 2st bag</p>
<p>now we need one more bag to put in the 3rd treasure.</p>
<p>This is not possible so u cant choose a bag of size 2</p>
<p>bag of size &gt;=3 can be used&nbsp;</p>
<p>Donn is intelligent and so he wants to pay the minimum cost so Donn will purchase a bag of size 3.Help Donn solve his problem .</p>
<p>&nbsp;</p>
<p>Input:</p>
<p>0&lt; T &lt;=100 ,no of test cases&nbsp;</p>
<p>Each test case contains</p>
<p>0&lt;N&lt;=1000,no of stages and then a space followed by</p>
<p>0&lt;k&lt;=1000, no of bags allowed</p>
<p>the next N lines contains the weights of the treasures in each stage<br>the weight of the treasure &lt;= 1000 .&nbsp;</p>
<p>output:</p>
<p>output a single line containing the minimum size of the bag needed.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>Example<span style="white-space:pre"> </span></p>
<p>Input:</p>
<p>1</p>
<p>3 2</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p>output :</p>
<p>3&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>