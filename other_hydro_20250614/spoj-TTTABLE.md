<p>A train line has two stations on it, A and B. Trains can take trips from A to B or from B to A multiple times during a day. When a train arrives at B from A (or arrives at A from B), it needs a certain amount of time before it is ready to take the return journey - this is the turnaround time. For example, if a train arrives at 12:00 and the turnaround time is 0 minutes, it can leave immediately, at 12:00.
<br><br>
A train timetable specifies departure and arrival time of all trips between A and B. The train company needs to know how many trains have to start the day at A and B in order to make the timetable work: whenever a train is supposed to leave A or B, there must actually be one there ready to go. There are passing sections on the track, so trains don't necessarily arrive in the same order that they leave. Trains may not travel on trips that do not appear on the schedule.

</p><h3>Input</h3>
<p>The first line of input gives the number of cases, <b>N(1&lt;=N&lt;=100)</b>. <b>N</b> test cases follow.

<br><br>
Each case contains a number of lines. The first line is the turnaround time, <b>T(0&lt;=T&lt;=60)</b>, in minutes. The next line has two numbers on it, <b>NA</b> and <b>NB</b>. <b>NA</b> is the number of trips from A to B, and <b>NB</b> is the number of trips from B to A<b>(0&lt;=NA,NB&lt;=100)</b>. Then there are <b>NA</b> lines giving the details of the trips from A to B.

<br><br>
Each line contains two fields, giving the HH:MM departure and arrival time for that trip. The departure time for each trip will be earlier than the arrival time. All arrivals and departures occur on the same day. The trips may appear in any order - they are not necessarily sorted by time. The hour and minute values are both two digits, zero-padded, and are on a 24-hour clock (00:00 through 23:59).

<br><br>
After these <b>NA</b> lines, there are <b>NB</b> lines giving the departure and arrival times for the trips from B to A.


</p><h3>Output</h3>
<p>For each test case, output one line containing "Case #x: " followed by the number of trains that must start at A and the number of trains that must start at B.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
5
3 2
09:00 12:00
10:00 13:00
11:00 12:30
12:02 15:00
09:00 10:30
2
2 0
09:00 09:01
12:00 12:02 

<b>Output:</b>
Case #1: 2 2
Case #2: 2 0 
</pre>