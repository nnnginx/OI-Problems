<p>Samuel has found a copy of a classic videogame called Crash Bandicoot!</p>
<p>Crash Bandicoot is a platform adventure videogame on which the player must complete levels by destroying crates and beating enemies. After completing successfully a level, the player is awarded with some prizes, such as crystals, gems and relics.</p>
<p>Samuel has already obtained all the crystal and gems of the game, and now he is aiming for the relics. A relic is obtained after completing successfully a Time-Trial challenge on a level.</p>
<p>However, Samuel knows there are two kinds of relics: Sapphire and Gold. Gold relics are harder to obtain than the sapphire ones, giving that the challenge must be completed going even faster.</p>
<p>When you start a Relic Challenge, the game tells you the maximum time you can expend in the level in order to obtain the sapphire relic, and after obtaining it, it tells you the gold relic time.</p>
<p>And Samuel has found a third hidden kind of relic even harder to obtain, the platinum relic! He wants to complete every challenge with this prize. However, Samuel doesn��t like to guess the time limit to obtain the platinum relic, so he hired you to find it quickly.</p>
<p>Your program must give the game a time in format hh:mm:ss:mss (hours, minutes, seconds and milliseconds respectively), where all the numbers, except hh, must have leading zeros. (By printing it in STDOUT)</p>
<p>Examples:<br> 0:04:57:987</p>
<p>2:14:08:057</p>
<p>Once you submit a time, the game will answer you with the relic you will win if you beat the level with that time.</p>
<p>For example, if the Relic challenges are:</p>
<p>Sapphire: 0:02:00:000</p>
<p>Gold: 0:01:35:000</p>
<p>Platinum: 0:01:00:000</p>
<p>And you submit 0:01:15:000, the game will answer "GOLD". If you submit 0:02:00:000 you will get "SAPPHIRE" and if you submit a time which surpass all the time limits, you will get "NO RELIC" as an answer.</p>
<p>When you have the answer, you must print "PLATINUM:", followed by a blank space, and then the maximum time Samuel can expend in order to obtain a platinum relic.</p>
<p>Some levels are absurdly long, so you must not make any assumption of how long a level can be.</p>
<h3>Input</h3>
<p>You will only receive the Sapphire time limit in the format explained above.</p>
<h3>Run Example</h3>
<p><strong>Game</strong>: 0:02:00:000</p>
<p><strong>You</strong>: 0:01:45:000</p>
<p><strong>Game</strong>: SAPPHIRE</p>
<p><strong>You</strong>: 0:01:15:000</p>
<p><strong>Game</strong>: GOLD</p>
<p><strong>You</strong>: 0:00:45:567</p>
<p><strong>Game</strong>: PLATINUM</p>
<p><strong>You</strong>: 0:01:00:000</p>
<p><strong>Game</strong>: PLATINUM</p>
<p><strong>You</strong>: PLATINUM: 0:01:00:000</p>
<p>&nbsp;</p>
<p>NOTE: <span style="color: #000020; font-size: 13px; text-align: justify; background-color: #f6f9e0;">the program should clear the output buffer after printing each line. It can be done using fflush(stdout) command or by setting the proper type of buffering at the beginning of the execution - setlinebuf(stdout).</span></p>