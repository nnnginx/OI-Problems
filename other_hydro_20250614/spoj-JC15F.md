<p><span style="font-size: x-large;"><strong>Colorful Beads</strong></span></p>
<p><img src="../../../content/tjandra:E_cover.jpg" alt=""></p>
<p>Yay, today is colorful day! why? because there are so many colorful beads on the table. Satria want to make a necklace using all that available beads, in order to make the necklace most valuable, Satria arrange the beads using magic secret formula. Gunawan secretly want to know Satria's secret formula, so he try all possible beads combination until the beads become most valuable, at first he easily found the most valuable beads combination for small number of beads, but he can't derive general formula, he keeps trying, and tying, and trying... Never give up!</p>
<p>Someday, Tjandra meet Gunawan and suggest him to not continuing his bruteforce action because the number of possible combinations are too many. Gunawan doesn't believe that and ask Tjandra to show him number of possible combinations.</p>
<p><span style="text-decoration: underline;">Gunawan said</span>: "If I have this N beads how many combinations are there?"<br><span style="text-decoration: underline;">Tjandra replied</span>: "It's N facorial combinations"<br><span style="text-decoration: underline;">Gunawan replied</span>: "But that's not always true some of my beads has more than one color, so if I swap beads with same color doesn't change tha necklace value"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Okay, tell me the details of your beads"<br><span style="text-decoration: underline;">Gunawan replied</span>: "My beads has M distinct colors, it has K<sub>1</sub> beads of color 1, K<sub>2</sub> beads of color 2, ... , K<sub>M</sub> beads of color M"<br><span style="text-decoration: underline;">Tjandra replied</span>: "It will have F(K<sub>1</sub>+K<sub>2</sub>+...+K<sub>M</sub>)/(F(K<sub>1</sub>)*F(K<sub>2</sub>)*...*F(K<sub>M</sub>)) combinations where F(N) means N factorial"<br>(5 minutes later)<br><span style="text-decoration: underline;">Gunawan said</span>: "Hey, your formula is not true, I tried it with 2 green beads and 2 blue beads, your formula showed F(2+2)/(F(2)*F(2)) = 24/(2*2) = 6 combinations, but actually it has only 2 combinations"<br><span style="text-decoration: underline;">Tjandra confidently replied</span>: "I'm good at math, I'm sure my formula is correct"<br><span style="text-decoration: underline;">Gunawan replied</span>: "I made these two different necklace: {1:{g,g,b,b},2:{g,b,g,b}} [g=green beads, b=blue beads] can you make the third necklace that is different than both of these?"<br><span style="text-decoration: underline;">Tjandra replied</span>: "That's easy, here is the third necklace: {b,g,b,g} "<br><span style="text-decoration: underline;">Gunawan replied after rotating that necklace</span>: "Look, your neclace become equal to my second necklace: {b,g,b,g} -&gt; {g,b,g,b}"<br><span style="text-decoration: underline;">Tjandra replied</span>: "Oops, I forgot about necklace rotation, you'really smart bruteforcer, why you don't believe me that number of combination is too many even though it's a little bit smaller than my calculation"<br><span style="text-decoration: underline;">Gunawan replied</span>: "A little bit? do you think 6 and 2 is little difference?"<br><span style="text-decoration: underline;">Tjandra replied</span>: "huh -_- I can show you that the exact number of distinct combinations, but unfortunately the formula become too complex and I don't bring a computer, is there any computer here?"<br><span style="text-decoration: underline;">Gunawan replied</span>: "No, I'm also don't have a computer"</p>
<p>Now Tjandra call you using his old phone for help, because he know that now you're sitting in front of your computer. Can you help them?</p>
<p><strong><span style="font-size: large;">Input</span></strong></p>
<p>The first line there is an integer K denoting number of distinct beads colors.<br>On the second line there are K integers, K<sub>i</sub>&nbsp;is number of beads with i-th color.</p>
<p><strong><span style="font-size: large;">Output</span></strong></p>
<p>Print single integer that is the number of distinct color combination. Since this number is very large as Tjandra predict, output it modulo 10<sup>9</sup>+7.</p>
<p><strong><span style="font-size: large;">Constraint</span></strong></p>
<p>1 ¡Ü&nbsp;K ¡Ü 1000</p>
<p>1 ¡Ü&nbsp;K<sub>i</sub> ¡Ü 1000</p>
<p><strong><span style="font-size: large;">Sample 1</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>1<br>1000</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>1</pre>
<p><strong><span style="font-size: large;">Sample 2</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>2<br>2 2</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2</pre>
<p><strong><span style="font-size: large;">Sample 3</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>3<br>1 1 1</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2</pre>
<p><strong><span style="font-size: large;">Sample 4</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>4<br>2 3 4 5</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>180180</pre>
<p><strong><span style="font-size: large;">Sample 5</span></strong></p>
<p><span style="text-decoration: underline;">Input</span></p>
<pre>5<br>1 2 3 4 5</pre>
<p><span style="text-decoration: underline;">Output</span></p>
<pre>2522520</pre>
<p><strong><span style="font-size: large;">Sample 3 Explanation</span></strong></p>
<p>On sample 3 there are 3 distinct color of beads, there is 1 bead for each color.</p>
<p>Let's assume those 3 distinct color are red, green, and blue,</p>
<p>here are 2 possible necklace, all other beads combination can be rotated to obtain one of thoose necklace below.</p>
<p><img src="../../../content/tjandra:sample3.png" alt=""></p>
<p>Note that if we can flip the necklace, both necklace are equal, but in this problem, we assume the front side of necklace is different than the back side, so both necklace above are considered different.</p>