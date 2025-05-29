<p>Beings (men) living on Mars discovered that there are beautiful beings (women) living on Venus.&nbsp; Men decided to change their life and want to travel using their spaceships to Venus to start a new life style. Unfortunately, women love connections and relationships and they won¡¯t let a group of spaceships pass to their planet unless the number of spaceships in one of the ¡°fully coupled¡± subgroups exceeds a certain minimum threshold. A fully coupled/connected group of spaceships is a group with each pair of spaceships can communicate together.</p>
<p>The spaceships and their airport on mars are very complicated. First, a spaceship communicates with another spaceship only if a command from the airport headquarter is issued. Second, the airport is a small one that can launch at a time a group of maximum K spaceships, connected in a random way. There are 2 types of commands that can be issued from headquarter to manage the spaceships connections: 1) <strong>Flip</strong> command for a group that establishes a new communication between every pair of disconnected spaceships and disconnect every previously connected pair of spaceships in the group, 2) <strong>Merge</strong> command for some of the groups to let them be <em>one group</em>, but no communications/connections modifications happen.</p>
<p>Unfortunately, under these constraints we can¡¯t launch all spaceships in a fully coupled state that satisfies women. So, the Men developed an automatic software that will issue commands to launch the spaceships in groups, then will issue commands (Flip, Merge) in a way that hopefully produces at least one of the fully connected subgroups with maximum number of spaceships that satisfies women so that they pass to Venus.</p>
<p>Given the groups of spaceships and the issued commands for them, you have to calculate the maximum number of spaceships that are fully coupled in <em>the final group</em>.</p>
<p><strong>Input Specification:</strong></p>
<p>The first line of input contains an integer T that represents the number of test cases, then follow T test cases. Each test case start with a line with N (the number of spaceships - 1 ¡Ü N ¡Ü 1000), M (the number of launch groups - 1 ¡Ü M ¡Ü 1000). Then M lines follow, one for each group: starting with K (number of spaceships in the group 1 ¡Ü K ¡Ü 10), E (number of connections in the group), and then E pair of numbers representing bidirectional connection between 2 spaceships: space_ship_id1, space_ship_id2 where 0 ¡Ü space_ship_id1, space_ship_id2 &lt; K. The m-th group has id (m-1).</p>
<p>Then Set of commands are given, each one on a line. Flip command on format ¡°<strong>F</strong> group_id¡± to flip the group with given group id. Merge Command on format ¡°<strong>M</strong> T group_id_1, group_id_2¡­ group_id_T¡± that merges T groups and let their <strong>new id</strong> to be the maximum id of the merged groups.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Output Specification:</strong></p>
<p>For each test case, output a single line of output in the form <strong>¡°Case K: T¡±</strong> where K is the number of the test case and T is the maximum number of spaceships that are fully coupled in the final group. Check sample below for the format.</p>
<p><strong>Sample input:</strong></p>
<p>1</p>
<p>7 4</p>
<p>3 3 0 1 0 2 1 2</p>
<p>2 1 0 1</p>
<p>1 0</p>
<p>1 0</p>
<p>F 1</p>
<p>M 2 1 2</p>
<p>F 0</p>
<p>M 2 0 2</p>
<p>F 2</p>
<p>M 2 3 2</p>
<p>*</p>
<p><strong>Sample Output:</strong></p>
<p>Case 1: 6</p>
<p><strong>Sample Explanation</strong></p>
<p>In this example we have 7 spaceships in 4 groups. First group (id = 0) is forming a triangle shape, second is segment shape, third is isolated spaceship and forth (id = 3) is also isolated. The first command flips the second group to 2 isolated spaceships. The second command merge 2 groups, id =2 to have 3 isolated spaceships with new. The third command flips first group to 3 isolated spaceships. The fourth one merges them under one group of 6 isolated group with id = 2. The fifth command flips this group to a fully coupled group of 6 spaceships. Finally a merge for that group with the fourth group and we have a new group with id = 3 of 6 spaceships fully connected and 1 isolated node.</p>