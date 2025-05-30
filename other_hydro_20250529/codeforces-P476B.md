## Description

<div><p>Dreamoon is standing at the position <span class="tex-span">0</span> on a number line. Drazil is sending a list of commands through Wi-Fi to Dreamoon's smartphone and Dreamoon follows them.</p><p>Each command is one of the following two types: </p><ol> <li> Go 1 unit towards the positive direction, denoted as <span class="tex-font-style-tt">'+'</span> </li><li> Go 1 unit towards the negative direction, denoted as <span class="tex-font-style-tt">'-'</span> </li></ol><p>But the Wi-Fi condition is so poor that Dreamoon's smartphone reports some of the commands can't be recognized and Dreamoon knows that some of them might even be wrong though successfully recognized. Dreamoon decides to follow every recognized command and toss a fair coin to decide those unrecognized ones (that means, he moves to the <span class="tex-span">1</span> unit to the negative or positive direction with the same probability <span class="tex-span">0.5</span>). </p><p>You are given an original list of commands sent by Drazil and list received by Dreamoon. What is the probability that Dreamoon ends in the position originally supposed to be final by Drazil's commands?</p></div><div class="input-specification"><p>The first line contains a string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> — the commands Drazil sends to Dreamoon, this string consists of only the characters in the set {<span class="tex-font-style-tt">'+'</span>, <span class="tex-font-style-tt">'-'</span>}. </p><p>The second line contains a string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> — the commands Dreamoon's smartphone recognizes, this string consists of only the characters in the set {<span class="tex-font-style-tt">'+'</span>, <span class="tex-font-style-tt">'-'</span>, <span class="tex-font-style-tt">'?'</span>}. <span class="tex-font-style-tt">'?'</span> denotes an unrecognized command.</p><p>Lengths of two strings are equal and do not exceed <span class="tex-span">10</span>.</p></div><div class="output-specification"><p>Output a single real number corresponding to the probability. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>


## Input

<p>The first line contains a string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> — the commands Drazil sends to Dreamoon, this string consists of only the characters in the set {<span class="tex-font-style-tt">'+'</span>, <span class="tex-font-style-tt">'-'</span>}. </p><p>The second line contains a string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> — the commands Dreamoon's smartphone recognizes, this string consists of only the characters in the set {<span class="tex-font-style-tt">'+'</span>, <span class="tex-font-style-tt">'-'</span>, <span class="tex-font-style-tt">'?'</span>}. <span class="tex-font-style-tt">'?'</span> denotes an unrecognized command.</p><p>Lengths of two strings are equal and do not exceed <span class="tex-span">10</span>.</p>


## Output

<p>Output a single real number corresponding to the probability. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>


## Samples

```input1
++-+-
+-+-+

```

```output1
1.000000000000

```






```input2
+-+-
+-??

```

```output2
0.500000000000

```






```input3
+++
??-

```

```output3
0.000000000000

```




## Note

<p>For the first sample, both <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> will lead Dreamoon to finish at the same position <span class="tex-span"> + 1</span>. </p><p>For the second sample, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> will lead Dreamoon to finish at position 0, while there are four possibilites for <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>: {<span class="tex-font-style-tt">"+-++"</span>, <span class="tex-font-style-tt">"+-+-"</span>, <span class="tex-font-style-tt">"+--+"</span>, <span class="tex-font-style-tt">"+---"</span>} with ending position {+2, 0, 0, -2} respectively. So there are <span class="tex-span">2</span> correct cases out of <span class="tex-span">4</span>, so the probability of finishing at the correct position is <span class="tex-span">0.5</span>. </p><p>For the third sample, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> could only lead us to finish at positions {+1, -1, -3}, so the probability to finish at the correct position <span class="tex-span"> + 3</span> is <span class="tex-span">0</span>.</p>

