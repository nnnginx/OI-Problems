<p>Usually, results of competitions are based on the scores of participants. However, we are planning a change for the next year of IPSC. During the registration each team will be able to enter a single positive integer : their preferred place in the ranklist. We would take all these preferences into account, and at the end of the competition we will simply announce a ranklist that would please all of you. </p>

<p>But wait... How would that ranklist look like if it won't be possible to satisfy all the requests? </p>

<p>Suppose that we already have a ranklist. For each team, compute the distance between their preferred place and their place in the ranklist. The sum of these distances will be called the badness of this ranklist. </p>

<h3>Problem specification</h3>
<p>Given team names and their preferred placements find one ranklist with the minimal possible badness. </p>

<h3>Input specification</h3>
<p>The first line of the input file contains an integer <b>T</b> specifying the number of test cases. Each test case is preceded by a blank line. </p>

<p>Each test case looks as follows: The first line contains <b>N</b> : the number of teams participating in the competition. Each of the next <b>N</b> lines contains a team name (a string of letters and numbers) and its preferred place (an integer between 1 and <b>N</b>, inclusive). No two team names will be equal. </p>

<h3>Output specification</h3>
<p>For each of the test cases output a single line with a single integer : the badness of the best ranklist for the given teams. </p>

<h3>Example</h3>
<pre><b>Input:</b>
2

7
noobz 1
llamas 2
Winn3rz 2
5thwheel 1
NotoricCoders 5
StrangeCase 7
WhoKnows 7

3
ThreeHeadedMonkey 1
MoscowSUx13 1
NeedForSuccess 1

<b>Output:</b>
5
3
</pre>

<b>Explanation:</b>
<p>In the first test case, one possible ranklist with the minimal badness is:</p>
<pre>1. noobz
2. llamas
3. Winn3rz
4. 5thwheel
5. NotoricCoders
6. WhoKnows
7. StrangeCase
</pre>
<p>In the second test case all ranklists are equally good.</p>
<b>Note: the input file will not exceed 5MB.</b>