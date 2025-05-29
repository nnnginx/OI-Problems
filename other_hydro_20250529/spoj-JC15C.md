<p><span style="font-size: large;"><strong>Walking Jumper</strong></span></p>
<p><img src="../../../content/tjandra:B_cover.jpg" alt=""></p>
<p>Gunawan really bored today, he sit in his home reading newspaper, but suddently he found very interesting news. Using modern radar, Satria detect a new chemical stone on top of the nearby mountain, the stone is so rare so it will be very valuable. After Gunawan know that news, he decided to climb that mountain to collect some of that valuable stone. To climb the mountain he need energy, to use energy he need oxygen, he know that when climbing the mountain there are some part of the mountain containing sulphuric gas and it's toxic so decreasing his oxygen, fortunately some other montain part containing clear breathable air that increasing his oxygen.</p>
<p>Because it's dangerous to climb the mountain without a map containing information about which part of the mountain has breathable air and which part of the mountain containing toxic sulphuric gas, Gunawan went to Tjandra house because Tjandra has that mountain map. Tjandra strongly advise Gunawan to take a deep breath before climbing this mountain to store some oxygen in his body and recommend him to train his jumping power to avoid the toxic gas part (by jumping of course).</p>
<p>After a few days of training, Gunawan observed that his optimal jumping power is propotional to the ammount of oxygen inside his body, that means if he has K unit of oxygen inside his body he can jump at most K unit skipping K-1 area that may be containing toxic gas. Not only that, he also obseved that after he jump his leg is shaking for a while so he must walk at some distance, this distance also the same as the distance he jumped, for example after he jump with distance K unit, he must walk K unit before he can make another jump. His last observation is that jumping has no effect with his oxygen inside his body, that means no matter how far he jump the ammount of oxygen in his body remain the same.</p>
<p>Tjandra tell Gunawan that he must keep his oxygen level positve, if he run out of oxygen (oxygen level in his body &lt;1) he will die. So Tjandra want to give Gunawan some oxygen supply, Tjandra know that pure oxygen is expensive this day so he must give the minimum possible oxygen that is enough to bring Gunawan to top of that mountain, also he also want the instruction (jump or walk plan) for Gunawan to use that oxygen wisely so he can reach the top of the mountain whithout running out of oxygen.</p>
<p>The objective is to keep the Gunawan from running out of oxygen, not nescesarily to maximize Gunawan's oxygen level at the top of the mountain. Tjandra know that you're very good at this kind of task so he call you using his old phone for your help. Can you help them?</p>
<p><span style="font-size: medium;"><strong>Input</strong></span></p>
<p>The first line there is an integer N denoting number of area in the map.<br>On the second line there is a string S of length N which is the content of that map.</p>
<p><strong><span style="font-size: medium;">Output</span></strong></p>
<p>On the first line you should output an integer that is the minimum number of oxygen that Gunawan needed at the beginning.<br>On the second line and after you sould output one instuction for each line, there are two types on instruction:</p>
<ul>
<li>If Gunawan need to walk to the next area, print a single character 'W' on that line</li>
<li>If Gunawan need to jump K unit (skipping K-1 area), print a single character 'J' and an integer K respectively on that line.</li>
</ul>
<p><strong><span style="font-size: medium;">Constraint</span></strong></p>
<p>1 ¡Ü N ¡Ü 1000</p>
<p>length of string S is equal to N, in other word: |S|=N</p>
<p>The first character of string S describing the area that is nearest to Gunawan's house, and the last character of string S describing the area that is nearest to the top of the mountain.</p>
<p>String S containing two possible characters:</p>
<ul>
<li>'+' means that area is a breathable area that increase Gunawan's oxygen level inside his body by one unit.</li>
<li>'-' means that area is a toxic sulphuric gas that decrease Gunawan's oxygen level inside his body by one unit.</li>
</ul>
<p><strong><span style="font-size: medium;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1<br>+</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1<br>W<br>W</pre>
<p><strong><span style="font-size: medium;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1<br>-</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2<br>J 2</pre>
<p><strong><span style="font-size: medium;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>5<br>-----</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>4<br>J 4<br>W<br>W</pre>
<p><strong><span style="font-size: medium;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>5<br>++---</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1<br>W<br>W<br>J 2<br>W<br>W</pre>
<p><strong><span style="font-size: medium;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>8<br>-+----+-</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>3<br>J 2<br>W<br>W<br>J 2<br>W<br>W<br>W</pre>
<p><strong><span style="font-size: medium;">Sample 5 Explanation</span></strong></p>
<p>If Gunawan has less than 3 unit of oxygen inside his body at the begining, he can't make it to the top of mountain, so the minimum number of oxygen needed is 3.</p>
<p>Here is the explanation of move command:</p>
<pre>[{3} G-+----+-_]</pre>
<p>: Initially Gunawan has 3 unit of oxygen inside his body.</p>
<pre>[{3} G-+----+-_] ="J 2"=&gt; [{4} _-G----+-_]</pre>
<p>: Gunawan jump 2 step forward to avoid the first toxic area, now he land on the breathable oxygen area increasing his oxygen level to 4.</p>
<pre>[{4} _-G----+-_] =="W"==&gt; [{3} _-.G---+-_]</pre>
<p>: Because Gunawan's leg is shaking after jump, he is unable to jump so his only choice is to walk to next area decreasing his oxygen level to 3 because that next area is toxic.</p>
<pre>[{3} _-.G---+-_] =="W"==&gt; [{2} _-..G--+-_]</pre>
<p>: Similar to his previous move, his only choice is to walk to the next area.</p>
<pre>[{2} _-..G--+-_] ="J 2"=&gt; [{1} _-...-G+-_]</pre>
<p>: After walking two steps his leg become normal again so he can jump to avoid the next toxic area, but unfortunately his remaining oxygen is only 2 so the best jump he can do is to jump 2 step forward landing on toxic area decreasing his oxygen level to 1.</p>
<pre>[{1} _-...-G+-_] =="W"==&gt; [{2} _-...-.G-_]</pre>
<p>: Fortunately the next area is breathable area, so he walk to this area increasing his oxygen level to 2.</p>
<pre>[{1} _-...-.G-_] =="W"==&gt; [{2} _-...-..G_]</pre>
<p>: Because the effect of previous jump is not gone, his leg is still shaking and his only choice is to move to the next area decreasing his oxygen value to 1 again.</p>
<pre>[{1} .-...-..G_] =="W"==&gt; [{1} .-...-...G]</pre>
<p>: Finally to reach the top of the mountain he need to walk once again and completed his mission</p>
<p>Don't worry about how Gunawan go home, because he is at the top of the tall mountain, to going home he simply jump of a cliff with his parachute :)</p>