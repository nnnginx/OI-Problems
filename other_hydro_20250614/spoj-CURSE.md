<p>Most of the contestants managed to arrive at the Benelux Algorithm Programming Contest on&nbsp;time. All except those unfortunate souls who chose to use a cheap car navigation system. A&nbsp;couple of wrong turns led them completely of course, and now they have ended up all over the&nbsp;world.&nbsp;Consider the case of contestant J.-P. B. (who has asked to remain anonymous). After driving&nbsp;for countless hours he found himself beneath three miles of water in the middle of the Atlantic&nbsp;Ocean. He was so focused on his navigation system that he failed to look outside until he noticed&nbsp;that the air was getting very moist. Fortunately for this contestant there was a spare submarine&nbsp;under his seat, which allowed him to escape this perilous situation.&nbsp;Tragic as this story seems, it is not even the worst. Another contestant, whom we will simply&nbsp;call S, wisely decided to travel by train. Sadly, she still listened to the advice of her evil car&nbsp;navigation system, and this morning she took a southbound train instead of heading north.&nbsp;After some more bad directions she found herself locked inside a labyrinth, in the pyramid of&nbsp;the Egyptian pharaoh Sok-O-Ban. As any experienced adventurer knows, these ancient tombs&nbsp;are often riddled with traps and other mechanisms. Sok-O-Ban's nal resting place was no&nbsp;exception.&nbsp;During his lifetime this pharaoh was known for his sadistic behavior, and he liked to give&nbsp;impossible challenges to random strangers. It is therefore no coincidence that the cavern where&nbsp;contestant S ended up was completely closed o, surrounded by solid rock on every side.&nbsp;After looking around, our protagonist S managed to draw a map of the tomb. Fortunately she&nbsp;found no skeletons, mummies or spiked death traps. She did discover some buttons embedded&nbsp;in the oor tiles. If she could press them all at the same time, then the hidden exit would open.&nbsp;But as soon as she would release one of the buttons, the door would close again.&nbsp;Besides the buttons, the walls and a few dusty oor tiles, there were also two sarcophagi lled&nbsp;with rocks. To accommodate the small stature of the ancient Egyptians, the sarcophagi were&nbsp;cubes with sides measuring 1 meter, the same size as the &nbsp;oor tiles. It seemed that these&nbsp;sarcophagi were the key to escaping: by pushing them onto the buttons the exit could be kept&nbsp;open. Only one small problem remained: the sarcophagi were far too heavy to move by hand&nbsp;and too large to climb over.&nbsp;Fortunately for S, the pharaoh did not anticipate the portable sarcophagus transporter she had&nbsp;conveniently stashed in her backpack. Attaching this reusable system to her arms allowed her&nbsp;to eortlessly push a sarcophagus exactly one meter straight ahead. This corresponds nicely to&nbsp;the 1 meter steps S used when marking out the grid in her map.</p>
<h3>Input</h3>
<p>On the first line of the input is a positive integer, the number of test cases. Then for each test&nbsp;case:&nbsp;A line containing two positive integers h;w  50, the height and width of the maze.&nbsp;h lines of w characters each, the map of the cavern our protagonist made, in which:&nbsp;'#' is a wall or otherwise impassible space.&nbsp;'.' is an empty space, of which there are at most 100.&nbsp;'S' is our protagonist.&nbsp;'X' is one of the heavy sarcophagi. There are at most two of these.'B' is a button. 'E' is the exit. There is exactly one exit, on the edge of the map.&nbsp;The edge of the map contains only walls and the exit.</p>
<h3>Output</h3>
<p>For each test case:&nbsp;One line containing the minimum number of steps2 it will take S to escape the tomb, or&nbsp;the text "impossible" if she cannot escape.</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
3
7 8
########
#..S...#
#.####.#
#.#.XB.#
#.####.#
#......E
########
7 8
########
#..S...#
#.####.#
#.#.BX.#
#.####.#
#......E
########
4 8
##E#####
#...####
#SX.XBB#
########

<strong>Output:</strong>
impossible
10
19</pre>