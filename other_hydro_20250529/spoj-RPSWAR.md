<p>The Danubian Lowland has always been a very fertile area. No wonder that a long, long time ago there were <strong>N</strong> kingdoms situated by the Danube river. As all good kingdoms do, each had chosen its favourite weapon,  which it equipped its armies with in times of war.</p>
<p>The Danube arsenal was quite limited - in these ancient times only three weapons were available: Rocketlaunchers, Pistols and Swords.  An army equipped with rocketlaunchers devastated those which challenged it with swords. At the same time, they did not stand a chance against opponents using pistols. And as you might already suspect, an army relying on pistols could not withstand the might of a sword-wielding army. Hence, we say that rocketlaunchers beat swords, swords beat pistols, and pistols beat rocketlaunchers.</p>
<p>Try to guess why the first two paragraphs were dedicated to kingdoms and their weapons. Exactly - these  kingdoms constantly fought against each other! Each kingdom went to war with both of its neighbours every year (respectively one, if the kingdom was the left or rightmost). Every war lasted exactly one year, after which the victorious kingdom captured one enemy territory. Of course, just after that another war began.</p>
<p>You are given a description of the kingdoms by the Danube river - <strong>N</strong> characters representing the chosen weapon of each kingdom - in the year 0. Each year, every kingdom will go to war with its neighbouring kingdoms. If two kingdoms <strong>a</strong> and <strong>b</strong> go to war, and the weapon of kingdom <strong>a</strong> beats the weapon of kingdom <strong>b</strong>, then at the end of the year kingdom <strong>a</strong> will capture one territory (one character) of kingdom <strong>b</strong>. If two kingdoms defeat the same territory of a kingdom at once, they decide which one captures the territory by a game of rock-paper-scissors.</p>
<p>After some finite number of years, there will only be a single weapon which all the remaining kingdoms are using. Find out which one.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>1 ¡Ü T ¡Ü 30</strong>: the number of test cases. <strong>T</strong> test cases follow.</p>
<p>For each case, the first line contains the integer <strong>1 ¡Ü N ¡Ü 10<sup>6</sup></strong> - the number of kingdoms by the Danube river. The second line contains <strong>N</strong> characters representing each kingdom's chosen weapon: <strong>R</strong> for rocketlaunchers, <strong>P</strong> for pistols, and <strong>S</strong> for swords.</p>
<p>The sum of <strong>N</strong> within one input file does not exceed <strong>2*10<sup>6</sup></strong>.&nbsp;</p>
<p><strong>Warning - the input is quite large. Make sure to read it efficiently.</strong></p>
<h3>Output</h3>
<p>For each test case, output "Case <strong>x</strong>: ", where <strong>x</strong> is the number of the test case, starting from 1, followed by the character <strong>R</strong>, <strong>P</strong> or <strong>S</strong>: the character representing the weapon which will conquer the entire river bank of Danube.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
RPS
7
RRRRRRP
<strong>Output:</strong>
Case 1: S
Case 2: P
</pre>
<p>In case 1, after the first year the situation will be PSS, and then after the second SSS.</p>
<p>In case 2, it will take the pistol-using kingdom six years, but no rocketlauncher-equipped kingdom will be able to stop it.</p>