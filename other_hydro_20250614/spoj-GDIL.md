<p><span style="font-size: small;"> </span></p>
<h1 lang="en-US"><span style="font-size: small;">&nbsp;</span></h1>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">Garfield  the cat likes candies A LOT. He always keeps a huge stock of it at his  home. Today John, his owner, brought home three types of candies.  He  brought A pieces of Red candy, B pieces of Green candy and C pieces of  Blue candy. Garfield is really happy. But the problem is that John won¡¯t  allow him to eat all of it at once. He will allow him to eat at most N  candies.  Garfield is very confused.  His love for candies is clouding  his judgement and he can¡¯t make a decision on how to choose the N  candies.</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">Garfield  is a dumb cat. So he asks you to find out in how many ways he can  choose from the available type of candies so that he eats a total of N  candies or less.</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">Note: There is no difference between candies of the same color</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><strong><span style="font-size: small;">Input:</span></strong></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><span style="font-size: small;">The first line contains an integer t, the number of test cases. Each test case contains four space separated integers N,A,B,C.</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><strong><span style="font-size: small;">Output:</span></strong></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><span style="font-size: small;">For each test case output a single line containing the number of ways Garfield can choose the N candies.</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><span style="font-size: small;"><strong>Constraints:</strong></span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US">&nbsp;</p>
<p lang="en-US"><span style="font-size: small;">0&lt;=t&lt;=100</span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">0&lt;=N,A,B,C&lt;=5000</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><span style="font-size: small;">** No other constraint applicable</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US">&nbsp;</p>
<p lang="en-US"><strong><span style="font-size: small;">SAMPLE INPUT:</span></strong></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">2 1 2 3</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">1 1 1 1</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">2 1 0 1</span></p>
<p lang="en-US"><strong><span style="font-size: small;"><br></span></strong></p>
<p><strong><span style="font-size: small;"> </span></strong></p>
<p><strong> </strong></p>
<p lang="en-US"><strong><span style="font-size: small;">SAMPLE OUTPUT:</span></strong></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">9</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">4</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">4</span></p>
<p lang="en-US"><span style="font-size: small;"><strong>SAMPLE TEST CASE EXPLANATION:</strong></span></p>
<p lang="en-US"><span style="font-size: small;"><strong><br></strong></span></p>
<p lang="en-US"><span style="font-size: small;">Explanation for the sample test case 1:</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;"><br></span><span style="font-size: small;">For the test case 2 1 2 3</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">There is 1 piece of Red candy, 2 pieces of Green and 3 pieces of Blue. Garfield can eat at most 2 candies.</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">the possible combinations are:</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(R,G,B)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,0,0)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,0,1)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,0,2)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,1,1)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(1,0,1)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,1,0)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(0,2,0)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(1,1,0)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">(1,0,0)</span></p>
<p><span style="font-size: small;"> </span></p>
<p lang="en-US"><span style="font-size: small;">&nbsp;</span><span style="font-size: small;">Therefore 9 is the answer.</span></p>