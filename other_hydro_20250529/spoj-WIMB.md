<p><span style="font-family: verdana,geneva;"><strong><span style="font-size: medium;">Problem:</span></strong></span></p>
<p><span style="font-family: verdana,geneva;"><span style="font-size: medium;">My boss hates me. He hates me to the extent where he plans meetings which clash with a Wimbledon match, almost all the time. Now, to give myself some inner peace, I decided to play well - while also trying to at least pray, that the matches I want to watch stretch enough for me to watch when I get back home. <br></span></span></p>
<p><span style="font-family: verdana,geneva;"> </span></p>
<p><span style="font-family: verdana,geneva;"><span style="font-size: medium;">But hey, wait! I may have a shot here! At Wimbledon, matches are played only at day light, so maybe if players were not ready to give up easily on each point, then the match will extend until sunset - just for my convenience! </span></span></p>
<p><span style="font-size: medium;">So what I need to know is how long on average a game between two players will last, and to help me feel better you should write a computer program to determine that!</span></p>
<p><span style="font-size: medium;"> </span></p>
<p>&nbsp;</p>
<p><span style="font-size: medium;"> </span></p>
<p>&nbsp;</p>
<p><span style="font-family: arial black,avant garde;"> </span></p>
<p><span style="font-family: verdana,geneva;"><span style="font-size: medium;">The result of a tennis match is determined by the number of ¡°sets¡± each player wins, the first player to win three sets wins the match. Accordingly, all possible match results are 3-0, 3-1 and 3-2. The result of each set is determined by the number of ¡°games¡± in the set each player wins, the first player to win six or more games with two or more game difference from the opponent wins the set, however if the result of a set (including the last set) leveled at 6-6 then a tie-break game is played to determine the set winner, Accordingly all possible set results are 6-0, 6-1, 6-2, 6-3, 6-4, 7-5 and 7-6 using a tie breaker game!</span></span></p>
<p><span style="font-family: verdana,geneva;"> </span></p>
<p><span style="font-family: verdana,geneva;"><span style="font-size: medium;">During each game (including tie-break), one player has the serve, this means that this player must start the play for all points of the game by hitting the ball, serving the ball is considered a big advantage. Assume that the serve starts at the first player and then alternates after each game till the end. Given the probability of winning a game on serve for each player against his opponent, and assuming that each game lasts for five minutes, calculate the expected duration of the match.<br></span></span></p>
<p><span style="font-family: verdana,geneva;"> </span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><span style="font-size: medium;"><span style="font-size: large;"><strong>Input:</strong></span><br></span></p>
<p>&nbsp;</p>
<p><span style="font-size: medium;">The first line of input contains an integer T, the number of test cases. The first line of each test case contains the first and last names of the first player, followed by an integer (0 &lt;= A &lt;= 100) where A/100 is the probability that the first player wins a game on his serve against the second player. The second line contains the first and last names of the second player, followed by an integer (0 &lt;= B &lt;= 100) where B/100 is the probability that the second player wins a game on his serve against the first player.</span></p>
<p>&nbsp;</p>
<p><strong><span style="font-size: large;">Output:</span></strong></p>
<p><span style="font-size: medium;">For each test case, print the duration of the match in minutes rounded to six decimal digits.</span></p>
<p>&nbsp;</p>
<p><span style="font-size: large;">Sample Input:</span></p>
<p><span style="font-size: medium;">2</span></p>
<p><span style="font-size: medium;">Pete Sampras 50</span></p>
<p><span style="font-size: medium;">Rafael Nadal 50</span></p>
<p><span style="font-size: medium;">Roger Federer 100</span></p>
<p><span style="font-size: medium;">Arjit Srivastava 0</span></p>
<p>&nbsp;</p>
<p><span style="font-size: large;"><strong>Sample Output:</strong></span></p>
<p><span style="font-size: medium;">199.281006</span></p>
<p><span style="font-size: medium;">90.000000</span></p>
<p>&nbsp;</p>
<h2><span style="font-size: medium;">How?</span></h2>
<p><span style="font-size: medium;">In the second test case, I don¡¯t stand a chance against Pete! He always wins all games on his serve (probability 100/100) and he also always wins all games on my serve (as I win with probability 0/100), so he always wins the match with three straight sets (6-0, 6-0, 6-0), a total of 18 games played, each lasting five minutes for a total of 90 minutes match.</span></p>