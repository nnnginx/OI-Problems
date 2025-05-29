<p><em>NOTICE</em>: The test cases for this problem are not as hard as intended. If you've solved this problem, and think your solution is up for it, try <a href="../VFRIEND2">VFRIEND2</a>!</p>
<p>You are creating a new soical network for dogs. Wow. The dogs don't have many possibilities for interacting with your website, but they can bark how many friends they want. E.g. if a dog wants to have much 8 friends it will bark 8 times, and if it doesn't want any friends, it'll just stay quiet.</p>
<p>After spending a good year of your life collecting these barks, you are finally ready to assign a friend list for each dog. The only problem is: You are not sure whether it is actually possible. Thus before you proceed you would like to write a program, that given a list of <strong>N</strong> wishes <strong>w<sub>i</sub></strong>, outputs <strong>HAPPY</strong> if it is possible to make a friend list for each dog <strong>i</strong> of length <strong>w<sub>i</sub></strong>, or <strong>SAD</strong> if some dog will have to get more or fewer friends than it wished for.</p>
<p>Notice: Being friends is considered an irreflexive, symetric relation.</p>
<p>Update: If you manage to solve this problem much efficiently, have a look at VFRIEND2, which is a so harder version of this problem.</p>
<h3>Input</h3>
<p>The first line will contain a single integer <strong>T</strong> - the number of test cases to process.</p>
<p>Each following lines will start with an integer <strong>0 ¡Ü N ¡Ü 10<sup>5</sup></strong> followed by an ordered list of <strong>N</strong> wishes <strong>0 ¡Ü w<sub>i</sub> ¡Ü 10<sup>5</sup></strong>.</p>
<h3>Output</h3>
<p>Write the answer - <strong>HAPPY</strong> or <strong>SAD</strong> - for each test case on a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>3 0 1 1<br>5 0 1 2 3 4<br>6 1 1 2 2 3 3

<strong>Output:</strong>
HAPPY<br>SAD<br>HAPPY</pre>
<h3>Explanation</h3>
<p>In the first case we can make dog 2 and 3 be friends.</p>
<p>In the second case no assignment that works, since dog 5 would have to be friends with everyone, but dog 1 doesn't want that.</p>