<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">is played with a deck of 24 cards: four labelled each of 1, 2, 3, 4, 5, 6. The cards in the deck are</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">visible to both players, who alternately withdraw one card from the deck and place it on a pile.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The object of the game is to be the last player to lay a card such that the sum of the cards in</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the pile does not exceed 31. Your task is to determine the eventual winner of a partially played</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">game, assuming each player plays the remainder of the game using a perfect strategy.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For example, in the following game player B wins:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player A plays 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player B plays 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player A plays 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player B plays 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player A plays 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player B plays 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The input will consist of several lines; each line consists of a sequence of zero or more digits</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">representing a partially completed game. The rst digit is player A's move; the second player</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">B's move; and so on. You are to complete the game using a perfect strategy for both players</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and to determine who wins.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For each game, print a line consisting of the input, followed by a space, followed by A or B to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">indicate the eventual winner of the game.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Example Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">356656</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">35665</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3566</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">111126666</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">552525</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Example Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">356656 B</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">35665 B</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3566 A</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">111126666 A</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">552525 A</div>
<p style="text-align: justify;">The game of 31 was a favourite of con artists who rode the railroads in days of yore. The game</p>
<p style="text-align: justify;">is played with a deck of 24 cards: four labelled each of 1, 2, 3, 4, 5, 6. The cards in the deck are</p>
<p style="text-align: justify;">visible to both players, who alternately withdraw one card from the deck and place it on a pile.</p>
<p style="text-align: justify;">The object of the game is to be the last player to lay a card such that the sum of the cards in</p>
<p style="text-align: justify;">the pile does not exceed 31. Your task is to determine the eventual winner of a partially played</p>
<p style="text-align: justify;">game, assuming each player plays the remainder of the game using a perfect strategy.</p>
<p style="text-align: justify;">For example, in the following game player B wins:</p>
<p>Player A plays 3</p>
<p>Player B plays 5</p>
<p>Player A plays 6</p>
<p>Player B plays 6</p>
<p>Player A plays 5</p>
<p>Player B plays 6</p>
<p><strong>Input:</strong></p>
<p>The input will consist of several lines; each line consists of a sequence of zero or more digits</p>
<p>representing a partially completed game. The rst digit is player A's move; the second player</p>
<p>B's move; and so on. You are to complete the game using a perfect strategy for both players</p>
<p>and to determine who wins.</p>
<p><strong>Output:</strong></p>
<p>For each game, print a line consisting of the input, followed by a space, followed by A or B to</p>
<p>indicate the eventual winner of the game.</p>
<p><strong>Example Input:</strong></p>
<p>356656</p>
<p>35665</p>
<p>3566</p>
<p>111126666</p>
<p>552525</p>
<p><strong>Example Output:</strong></p>
<p>356656 B</p>
<p>35665 B</p>
<p>3566 A</p>
<p>111126666 A</p>
<p>552525 A</p>
<p>&nbsp;</p>
<p>&nbsp;</p>