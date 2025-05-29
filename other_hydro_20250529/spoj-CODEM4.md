<p>"Roadies" is back!!! In India,"Roadies" is a reality based tv show and is very popular among the youth.</p>
<p>This time to get selected into "Roadies" they challenge you to solve the given problem....if you can solve it you will be selected!</p>
<p>Challenge is as follows: Suppose you are given an array with even number of integers.Player 1 and player 2 take turns to pick numbers,either the leftmost element or the rightmost element.You have to find the maximum possible score (sum of numbers chosen) by player 1.Assume player1 always starts the game and plays optimally.</p>
<p><strong>Note</strong>:when an element is picked it is removed from the array.</p>
<p>But as usual this is "Roadies" hence cometh the twist.It is not known whether the second player plays like a dumb or smart.As you know result will be different if player 2 is either dumb or smart.</p>
<p><strong>NOTE:</strong> when player 2 plays like a dumb <span style="text-decoration: underline;">there is no fixed strategy of how he would choose the numbers</span> i.e he would choose the number either from start or end of an array without thinking...so there can be multiple answers possible when player 2 plays like a dumb...</p>
<p><strong>So you have to tell the maximum possible score of player 1 when player 2 plays like a dumb and smart.</strong></p>
<p><strong>Input description:</strong><span style="font-weight: bold;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 69px; width: 1px; height: 1px; overflow: hidden;"><strong>T:no of test cases(t&lt;20)</strong></div>
<p><strong> </strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 69px; width: 1px; height: 1px; overflow: hidden;"><strong>For eact case two lines follow,first line contains the size of array(&lt;=30) and next line contains elements of array.</strong></div>
<p>T:no of test cases(t&lt;20)</p>
<p>For eact case two lines follow,first line contains the size of array(&lt;=30) and next line contains elements of array.</p>
<p><span style="font-weight: bold;">Output description:</span></p>
<p>For each case print in new line two space separated integers: score when player 2 is dumb and score when player 2 is smart.</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>2</p>
<p>4</p>
<p>5 8 4 2</p>
<p>4</p>
<p>8 5 4 2</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>13 10</p>
<p>13 12</p>
<p>&nbsp;</p>
<p><strong>NOTE</strong>:All values will fit in int type.</p>
<p><strong>Explanation</strong>:In first test case (when player 2 is dumb) then player 1 first chooses 5 then player 2 can choose 8 or 2 but chooses 2. so now player 1 can choose either 8 or 4 so chooses 8.Hence total score is 13.&nbsp;</p>
<p>(when player 2 is smart) player 1 can choose 5 or 2 but chooses 2(so that player 2 cannot choose 8 in his turn) so now player 2 can choose 5 or 4.Irrespective of what player 2 chooses player 1 will have option to choose 8 in his next turn hence total (8+2)=10.</p>