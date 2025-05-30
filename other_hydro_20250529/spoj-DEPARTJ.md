<p style="text-align: justify;">The Department of Security has a new headquarters building. The building has several floors, and on each floor there are rooms numbered&nbsp;<em>xxyy</em>where&nbsp;<em>yy</em>&nbsp;stands for the room number and&nbsp;<em>xx</em>&nbsp;for the floor number, 0 &lt;&nbsp;<em>xx</em>,&nbsp;<em>yy</em>&nbsp;&lt; 10.</p>
<p style="text-align: justify;">The building has "pater-noster" elevator, i.e. elevator build up from several cabins running all around.From time to time the agents must visit the headquarters.During their visit they want to visit several rooms and in each room they want to stay for some time. Due to the security reasons, there can be only one agent in the same room at the same time, The same rule applies to the elevators.</p>
<p style="text-align: justify;">The visits are planned in the way ensuring they can be accomplished within one day. Each agent visits the headquarters at most once a day.</p>
<p style="text-align: justify;">Each agent enters the building at the 1st floor, passes the reception and then starts to visit the rooms according to his/her list. Agents always visit the rooms by the increasing room numbers. The agents form a linear hierarchy according to which they have assigned their one letter personal codes. The agents with higher seniority have lexicographically smaller codes. No two agents have the same code.</p>
<p style="text-align: justify;">If more then one agent want to enter a room, or an elevator, the agents have to form a queue. In each queue, they always stand according to their codes. The higher the seniority of the agent, the closer to the top of the queue he stands. Every 5 s (seconds) the first agent in the queue in front of the elevator enters the elevator. After visiting the last room in the headquarters each agent uses if necessary elevator to the first floor and exits the building.</p>
<p style="text-align: justify;">The times necessary to move from a certain point in the headquarters to another are set as follows: Entering the building, i.e. passing the reception and reaching the elevator, or a room on the first floor takes 30 s. Exiting the building, i.e. stepping out of the elevator or a room on the first floor and passing the reception takes also 30 s. On the same floor, the transfer from the elevator to the room (or to the queue in front of the room), or from the room to the elevator (or to the queue in front of the elevator), or from one room to another (or to the queue in front of the room) takes 10 s. The transfer from one floor to the next floor above or below in an elevator takes 30 s. Write a program that determines time course of agent's visits in the headquarters.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001001000000000000000">Input</a></span></h2>
<p style="text-align: justify;">The input file contains the descriptions of&nbsp;<img src="./22130/file/WBcE9hII.png" alt="tex2html_wrap_inline49" width="41" height="25" align="MIDDLE">&nbsp;visits of different agents. The first line of the description of each visit consists of agent's one character code&nbsp;<em>C</em>,&nbsp;<em>C</em>&nbsp;=&nbsp;<tt>A, ..., Z</tt>, and the time when the agent enters the headquarters. The time is in the format HH:MM:SS (hours, minutes, seconds). The next lines (there will be at least one) contain the room number, and the length of time intended to stay in the room, time is in seconds. Each room is in a separate line. The list of rooms is sorted according to the increasing room number. The list of rooms ends by the line containing 0. The list of the descriptions of visits ends by the line containing the character dot.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001002000000000000000">Output</a></span></h2>
<p style="text-align: justify;">The output contains detailed records of each agent's visit in the headquarters. For each agent, there will be a block. Blocks are ordered in the order of increasing agent's codes. The first line of a block contains the code of agent. Next lines contain the starting and ending time (in format HH:MM:SS) and the descriptions of his/her activity. Time data will be separated by one blank character. Description will be separated from time by one blank character. Description will have a form&nbsp;<tt>Entry, Exit</tt>&nbsp;or Message. The Message can be one of the following:&nbsp;<tt>Waiting in elevator queue, Waiting in front of room</tt>&nbsp;<em>RoomNumber</em>,&nbsp;<tt>Transfer from room</tt>&nbsp;<em>RoomNumber</em>&nbsp;<tt>to room</tt>&nbsp;<em>RoomNumber</em>,<tt>Transfer from elevator to room</tt>&nbsp;<em>RoomNumber</em>,&nbsp;<tt>transfer from</tt>&nbsp;<em>RoomNumber</em>&nbsp;<tt>to elevator</tt>,&nbsp;<tt>Stay in room</tt>&nbsp;<em>RoomNumber</em>,&nbsp;<tt>Stay in elevator</tt>.<br>Print a blank line after each block.</p>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001003000000000000000">Sample Input</a></span></h2>
<pre>A 10:00:00
0101 100
0110 50
0202 90
0205 50
0
B 10:01:00
0105 100
0201 5
0205 200
0
.</pre>
<p>&nbsp;</p>
<h2><span style="color: #000000;"><a name="SECTION0001004000000000000000">Sample Output</a></span></h2>
<pre>A
10:00:00 10:00:30 Entry
10:00:30 10:02:10 Stay in room 0101
10:02:10 10:02:20 Transfer from room 0101 to room 0110
10:02:20 10:03:10 Stay in room 0110
10:03:10 10:03:20 Transfer from room 0110 to elevator
10:03:20 10:03:50 Stay in elevator
10:03:50 10:04:00 Transfer from elevator to room 0202
10:04:00 10:05:30 Stay in room 0202
10:05:30 10:05:40 Transfer from room 0202 to room 0205
10:05:40 10:07:40 Waiting in front of room 0205
10:07:40 10:08:30 Stay in room 0205
10:08:30 10:08:40 Transfer from room 0205 to elevator
10:08:40 10:09:10 Stay in elevator
10:09:10 10:09:40 Exit

B
10:01:00 10:01:30 Entry
10:01:30 10:03:10 Stay in room 0105
10:03:10 10:03:20 Transfer from room 0105 to elevator
10:03:20 10:03:25 Waiting in elevator queue
10:03:25 10:03:55 Stay in elevator
10:03:55 10:04:05 Transfer from elevator to room 0201
10:04:05 10:04:10 Stay in room 0201
10:04:10 10:04:20 Transfer from room 0201 to room 0205
10:04:20 10:07:40 Stay in room 0205
10:07:40 10:07:50 Transfer from room 0205 to elevator
10:07:50 10:08:20 Stay in elevator
10:08:20 10:08:50 Exit</pre>