<p><em>Original problem statement (in Polish) can be found <a href="https://pizza.natodia.net/static/tasks/2015/eliminations/kontruderzenie.pdf">here</a>.</em></p>
<p>Januarius the Clairvoyant recently started playing the popular, team-based online video game - Counter-Smack. His paranormal abilities are certainly a big help during the gameplay, but even having a keen inner eye is not enough when all of your teammates are total noobs. There's just no way to climb up the ranking when something like this happens.</p>
<p>Counter-Smack's ranking system is really simple. The player starts with zero points. For every win he gains a point, for every defeat he loses a point. Of course the more points, the better.</p>
<p>One may think that using the gift of clairvoyance you could detect the noobs in advance, and just skip the game in case they would join your team. Unfortunately, that's not how the laws of the universe work, and Januarius knows that. As it turns out, team-based online games are one of the few cases where the Primeval Law of Destiny applies - it may just so happen that you will be joined by noobs in the next game and you can't do anything about it, as it is already written down in the Universum's atoms.</p>
<p>Fortunately, there is a loophole. You can join the game and immediately leave, and the destiny will be fulfilled. Even though you lose a point for leaving the game (just as in the case of simply losing), you are additionally banned for a few next games - and being banned also fulfills the destiny.</p>
<p>Using his abilities, Januarius can predict the future for the next <strong>n</strong> games - he will know whether he will be joined by the noobs or not. When leaving the game for the first time, the player is banned for the next one. Leaving for the second time will get you banned for the next two games. Leaving for the third time results in a ban that lasts for four games, and so on - every ban is twice as long as the previous one.</p>
<p>What is the maximum number of points Januarius can achieve in <strong>n</strong> succesive games, if he starts with zero points, he wins every match without the noobs on his team, and loses all the other matches?</p>
<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, testcases follow, each in a separate line.</p>
<p>Each testcase consists of a string of length <strong>n</strong>, describing the predicted future for the next <strong>n</strong> games. (1 &lt;= <strong>n</strong> &lt;= 2*10<sup>5</sup>). i-th letter indicates the i-th game. "N" means that Januarius will be joined by the noobs in this game, "P" denotes good players.</p>
<h3>Output</h3>
<p>For each testcase you should output a single integer - the maximum number of ranking points that Januarius can achieve by abandoning some of the matches.</p>
<h3>Example</h3>
<p>Input:</p>
<pre>4
PPPPP
PPPPN
NNPPP
NNNNN</pre>
<p>Output:</p>
<pre>5
3
2
-2</pre>
<h3>Explanation</h3>
<p>In the third testcase, by abandoning the first game, Januarius will be banned for the next one. He will win the rest of them, so his final result will be (-1)+3 = 2 points.</p>
<p>In the fourth testcase, Januarius can abandon the first game, which will get him banned for the next one. Then he can abandon another game, and this time he will get banned for the last two games. His final score will be -2 points, for abandoning two games.</p>