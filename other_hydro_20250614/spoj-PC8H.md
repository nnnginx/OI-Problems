<p>RoboCorp Oregon has already deployed several of its PoliceBots throughout the state, and suddenly they have remembered the importance of being able to repair these bots when they break. They are willing to build only a limited number of repair depots in the state, and they want to locate these depots so that each PoliceBot's city is within a given distance of some depot. You are given the locations of where the n (1 ¡Ü n ¡Ü 16) PoliceBots have been deployed, and the maximum number (1 ¡Ü c ¡Ü n) of repair depots that RoboCorp is willing to construct. Your job is to locate these repair depots to minimize the distance any bot has to be transported for repair, and return what that maximum distance is. You can assume that any bot can be repaired at any depot.</p>
<h3>Input</h3>
<p>The first line contains the integer t (1 ¡Ü t ¡Ü 350), the number of cases. Each case starts with a line containing n and c. Following this line is one line per deployed bot; that line contains two floating point values, separated by a single space, giving the Cartesian coordinates of the bot. Each such value will be between 0.0 and 10.0, inclusive (NOTE: the Sample Input shows integer values for brevity).</p>
<h3>Output</h3>
<p>You are to print for each input set the minimum value that can be obtained, such that each PoliceBot is within that distance of some depot. You should print your result with at least one digit before and exactly six digits after the decimal point; your value should be within 5e-7 of the true result. To make round-off error less of a concern, the true result will never have a 4 or a 5 as the seventh digit after the decimal point.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
9 3
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
4 2
0 0
1 1
2 4
3 9
</pre>

<pre><strong>Output:</strong>&nbsp;
1.000000
2.236068
</pre>