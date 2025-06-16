<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>In a certain peaceful forest, there live a Fox and a Wolf. Due to common misconception, one might suppose that the Wolf would want to hunt the Fox �C however, both are in fact nice animals, and get along just fine. Indeed, they have such nice manners that, if they ever meet up, they will have a nice little chat for $C$ minutes&nbsp;($1 \leq C \leq 9$).</p>
<p>The forest that the Fox and the Wolf live in can be regarded as a rectangle, $N$&nbsp;km long along its East side and $M$ km wide along its North side ($1 \leq N,M \leq 20$). It is divided into a grid of squares, each with a side length of 1 km. Each such square either contains a meadow (represented by a ��.��), is full of burrs (��B��), is blocked by trees (��T��), contains the Fox��s den (��F��), contains the Wolf��s lair (��W��), currently contains the Fox (��f��), or currently contains the Wolf (��w��).</p>
<p>At the end of a long day at work (consisting of solving complex computer science problems in their heads), both animals wish to get to their respective homes as soon as possible. Every minute, each of them can walk one km directly North, East, South, or West, or just stay put �C however, they cannot enter squares blocked by trees, nor can they enter each other��s homes (that wouldn��t be very polite). They also don��t want to leave the forest, seeing as humans jealous of their supreme intellect are constantly lurking just outside.</p>
<p>Every time the Fox or the Wolf goes from a square full of burrs to a meadow, he must stand still and spend $B$&nbsp;minutes ($1 \leq B \leq 9$) picking burrs off of himself. As mentioned above, they must also stop and chat if they meet up. Though each square is quite big, the animals always walk to its exact centre before moving on. This means that they will meet up if they either occupy the same square at the same time, or if they pass each other while walking between squares (which would happen if they switched positions in the space of a minute). Once the animals have chatted once, they never have to chat again, having already satisfied the demands of etiquette. Both animals are great multitaskers, and can pick burrs while chatting with each other.</p>
<p>Each animal wants to get home as soon as possible, but is also considerate of the other �C as such, they will collaborate so as to minimize the time for both of them to get home. Due to their extreme intelligence, both animals will calculate this minimum time in their heads instantly �C however you, the observer, will probably need to write a program to figure it out...</p>
<h3>Input</h3>
<p>Line $1$: 4 integers, $N$, $M$, $C$, and $B$</p>
<p>Next $N$&nbsp;lines: $M$&nbsp;characters each, representing a row of the forest as described above</p>
<h3>Output</h3>
<p>A single integer �C the minimum time for both the Fox and the Wolf to get to their respective homes, in minutes. If this is impossible, output -1 instead.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">5 6 5 1</span>
<span style="font-family: 'courier new', courier;">......</span>
<span style="font-family: 'courier new', courier;">BWTTTB</span>
<span style="font-family: 'courier new', courier;">B.TB..</span>
<span style="font-family: 'courier new', courier;">BBT..T</span>
<span style="font-family: 'courier new', courier;">.FTfw.</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">17</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The Wolf should wait for the first three minutes, letting the Fox go first. From then on, the Fox can continue along its only possible route home. The Wolf will be 2 squares behind the Fox most of the time, except for when it enters the burr-filled square, when it will temporarily be 1 behind. With this strategy, the Wolf will take 14 minutes to get home, while the Fox will take 17, and since we only care about the larger, the total time is 17 minutes.</p>