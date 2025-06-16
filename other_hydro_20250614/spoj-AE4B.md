<p>Byteman woke up early this morning, just after dawn. He is planning to get to the top of Bytemountain, so
the spent the night in a mountain hostel right in the middle of picturesque mountain range of Lower Bytehills.
Since Bytemountain in the highest mountain of the range, at each trail crossing there is a signpost pointing
at the trail leading towards its peak.</p>
<p>In the mountain hostel Byteman met a guide who knows Lower Bytehills like the back of his hand. The
guide informed Byteman that the signposts are being reorganized and because of that he should not rely too
much on the signposts. In particular, the very peak of Bytemountain is also a crossing and at this crossing
there is a signpost pointing to some trail ※leading§ to Bytemountain!</p>
<p>The guide will explain Byteman how to get to the peak. Luckily, all trail crossings are numbered from 1
to n and each crossing contains a tablet with the number of the crossing written on it. The guide＊s directions
will have the following form: ※Walk along the trails pointed by the signposts until you reach crossing s<sub>1</sub>, then
take a map and choose the trail connecting crossing s<sub>1</sub> with crossing c<sub>1</sub>. Afterwards keep walking along the
trails pointed by the signposts until you reach crossing s<sub>2</sub>. The take a look at the map and choose the trail
connecting s<sub>2</sub> and c<sub>2</sub>. . . Finally, when you reach s<sub>i</sub>, take the last look at the map and walk along the trail
connecting s<sub>i</sub> and c<sub>i</sub>. If you keep walking along the trails pointed by the signposts since then, you will reach
the peak of Bytemountain.§</p>
<p>Byteman would not like the description of the route to be too complicated, so he asked the guide for a route
that would not require looking at the map more than k times.</p>
<p>The guide had to take a deeper thought, because he knows that some trails are more exciting than others
and he would like to show Byteman the most interesting route.</p>
<p>The route may lead through the same trails and crossing many times (some trails are so exciting that they
may be worth visiting multiple times!)</p>
<p>Byteman ends his walk when he reaches the peak for the first time after using all instructions provided by
the guide. This means that Byteman can visit the peak of Bytemountain multiple times during the walk, but
he will end his walk only after all instructions have been used.</p>
<p>How interesting can the route provided by the guide be?</p>

<h3>Input</h3>
<p>The first line of the standard input contains two integers n and k (1 ≒ n ≒ 50000, 0 ≒ k ≒ 100) separated by
a single space. They denote the number of trail crossings and the maximum number of times Byteman would
like to look at the map. The crossings are numbered from 1 to n, the mountain hostel is located at crossing 1,
and the peak of Bytemountain is the crossing number n.</p>

<p>The following n lines contain descriptions of the respective trail crossings. Each crossing＊s description
consists of a single line and is composed of integers separated by single spaces. The first one of these numbers, m<sub>i</sub> (1 ≒ m<sub>i</sub> ≒ n-1), denotes the number of trails going out of the crossing. After that there are m<sub>i</sub> pairs of numbers a<sub>i,j</sub> , b<sub>i,j</sub> (1 ≒ a<sub>i,j</sub> ≒ n, 1 ≒ b<sub>i,j</sub> ≒ 10000), meaning that from the ith crossing there is a trail leading to
crossing a<sub>i,j</sub> with beauty equal to b<sub>i,j</sub> . The first pair of numbers denotes the trail that leads to Bytemountain
according to the signpost at the crossing. Each trail is bidirectional and connects two different crossings. Each
two crossings can be connected by at most one trail. The total number of all trails does not exceed 100000.</p>

<p>Each trail connecting crossings i and j will appear in the input twice: first time in the list of trails going
out of the i<sup>th</sup> crossing and second time in the list of trails going out of the j<sup>th</sup> crossing. In both cases the
beauty of the trail will be the same.</p>
<h3>Output</h3>
<p>The first and only line of the standard output should contain a single integer denoting the maximum possible
sum of beauties of consecutive trails on the route from the mountain hostel to the peak of Bytemountain that
satisfies Byteman＊s requirements. You can assume that there exists at least one such route.</p>
<h3>Example</h3>
<p>For the input data:</p>
<pre>5 2
2 3 4 2 2
3 1 2 5 4 4 3
2 1 4 4 3
3 2 3 5 5 3 3
2 2 4 4 5
</pre>
<p>the correct result is:</p>
<pre>14</pre>

<img src="./21264/file/pdQb3cVI.png">


<p>Explanation of the example. In the above figure the edges represent trails connecting respective crossings,
the numbers next to the edges 〞 the beauties of the trails, and the arrows denote the trails pointed by the
signposts at respective crossings.</p>
<p>The guide will ask Byteman to look at the map twice, at crossings number 3 and 2. This way Byteman＊s
walk will lead along the route 1 每 3 每 4 每 2 每 5. The total beauty of the trails on this route is 14.</p>