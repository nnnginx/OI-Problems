<p>In the local pond there are <strong>n</strong> lillypads arranged in a row - frog households - numbered <strong>1</strong> to <strong>n</strong> from left to right. One frog lives on each lillypad. In the afternoon, each frog returns to its household for a short nap. After they wake up from their naps, it is already evening. And what do frogs do on evenings? They throw a party! Luckily, a frog party doesn't require any special preparations - all the frogs simply meet up at a single lillypad, and the fun may begin.</p>
<p>When a frog goes to a party, it definitely doesn't want to arrive wet. Hence, frogs may only travel to  the party by jumping across lillypads. A single frog by itself can jump to a neighbouring lillypad. However, when a frog jumps to a lillypad with another frog on it, they team up - the frog that arrived jumps on the other's back, and with combined efforts (and slightly defying the laws of physics) they can jump to a lillypad which is at a distance of <strong>2</strong>. In general, if there are <strong>y</strong> frogs on the lillypad numbered <strong>x</strong>, they can jump to lillypads with numbers <strong>x-y</strong> and <strong>x+y</strong> (jumping outside the <strong>n</strong> lillypads is obviously forbidden - the frogs would jump into the water and get wet). When frogs from one lillypad jump onto another, they climb on the backs of the frogs which were already present, in the same order as before. On top of that, polite frog manners say that frogs should not jump on a lillypad on which there are currently no frogs.</p>
<p>The whole process might look like this</p>
<p><img src="./22487/file/4Qigb40J.png" alt="" width="624" height="114"></p>
<p><img src="./22487/file/gOyj6sZi.png" alt="" width="622" height="140"></p>
<p><img src="./22487/file/PxYiCwUY.png" alt="" width="623" height="170"></p>
<p><img src="./22487/file/j37dBUqF.png" alt="" width="622" height="213"></p>
<p><img src="./22487/file/oC51ZXrn.png" alt="A frog party" width="626" height="207"></p>
<p>As you can imagine, when several frogs stand on another's back, it can be quite tiring. Frog Michal obviously doesn't want to do activities which are tiring. That's why he would like to propose a sequence of jumps at the next frog meeting, such that in the evening all frogs will end up meeting on one lillypad, and at the same time no frog ever climbed on Michal's back (that basically means that no frog can ever jump to the lillypad on which Michal is currently situated).  Help him!</p>
<p>Given the number of lillypads <strong>n</strong> and the number of lillypad on which Michal lives, produce a sequence of jumps so that all frogs end up on a single lillypad, and no frog ever jumps on a lillypad which currently has no frogs on it, or has frog Michal on it.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü&nbsp;</strong><strong>T ¡Ü 60</strong>: the number of testcases.</p>
<p>For each testcase, in the only line of input there are two whole numbers <strong>n </strong>and <strong>m</strong>,&nbsp;<strong>1 ¡Ü m ¡Ü n ¡Ü 10<sup>6</sup></strong>: the number of lillypads (and frogs), and the number of the lillypad on which Michal lives.</p>
<p>The sum of <strong>n</strong>&nbsp;within a single input file does not exceed <strong>2*10<sup>6</sup></strong>.</p>
<h3>Output</h3>
<p>For each testcase, if no valid sequence of jumps which fulfills the criteria described exists, output "NO". Otherwise in the first line output "YES", and then describe a valid sequence of jumps. Each jump can be described by two numbers <strong>1 ¡Ü&nbsp;a,b ¡Ü&nbsp;n</strong>, meaning that the frogs currently on lillypad <strong>a</strong> should jump to the lillypad <strong>b</strong>. Any valid sequence of jumps leading to a frog party will be accepted.</p>
<p>The output is very large. Please be wary of your I/O speed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 4
9 3
</pre>
<pre><strong>Output:</strong>
YES
2 3
3 5
4 5
5 1 
YES
1 2
3 2
4 5
6 5
7 8
9 8
8 5
2 5
</pre>
<p>The first case is depicted in the images in the problem text.</p>