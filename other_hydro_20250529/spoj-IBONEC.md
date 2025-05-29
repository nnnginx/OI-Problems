<p>The International beuro of epidemic control has recently found a weird virus which is spreading very rapidly. The infection of this virus happens in a very peculiar way. To any healthy person, it needs 4 infected people to get infected to. While infecting each virus splits into two; First half remains to the infecting guy and other one goes to the healthy guy. This way the newly infected guy gets total viruses equal to all those 4 infected people.</p>
<p>However, due to immunity of body some viruses die immediately. It has been found that the number of viruses dying due to immunity is always equal to the second least number of viruses recieved from the four infecting people. That means, if four infecting people have v1, v2, v3 and v4 viruses and v1 &lt;= v2 &lt;= v3 &lt;= v4, then the healthy guy will ultimately have v1 + v3 + v4 viruses remaining in the body. After that, this number remains constant in the body. Strangely, this epidemic does not spread as other epidemics. The infected person with least viruses (here v1) will no longer infect any other person. Also, once infected person cannot be infected again.</p>
<p>The beuro has identified that this virus is very lethal as it's population is increasing very rapidly. They have discoverd a vaccine which costs 1$ to kill 1 virus. Since, it is an international beuro, they can afford this cost for the cause of humanity. But they need to know first, how much would it cost in total to get rid of this virus forever, given that N people have already been infected by this virus.</p>
<p>You have been asked by this beuro to compute the total number of viruses spread among the world. Oh yes, this infection was started by four culprits who went on a tour in a jungle and ate up some hyenas there. When these four came back from the tour, they had 1, 2, 3 &amp; 5 viruses in their bodies respectively.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line contains a positive integer T (T ¡Ü&nbsp;1000). Then T lines follows, each line containing one positive integer N (4 ¡Ü&nbsp;N ¡Ü&nbsp;10<sup>10</sup>).</p>
<h3>Output</h3>
<p>For each test case print total number of viruses spread in the world, given that total N people has been infected. Since, this can be very huge number, print modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>5<br>6<br>100</pre>
<pre><strong>Output:</strong>
20<br>36<br>639154830</pre>
<h3>Explanation:</h3>
<p>For first test N = 5. Given that V1 = 1, V2 = 2, V3 = 3, V4 = 5 and V5 = V4 + V3 + V1 = 9 because V2 viruses died immediately after infection. Thus, total viruses in the world are: <br>(1 + 2 + 3 + 5 + 9) = 20.</p>