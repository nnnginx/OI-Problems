<p>County General Hospital is trying to chart its course through the troubled waters of the economy and shifting population demographics. To support the planning requirements of the hospital, you have been asked to develop a simulation program that will allow the hospital to evaluate alternative configurations of operating rooms, recovery rooms and operations guidelines. Your program will monitor the usage of operating rooms and recovery room beds during the course of one day.</p>
<p>
County General Hospital has several operating rooms and recovery room beds. Each surgery patient is assigned to an available operating room and following surgery the patient is assigned to one of the recovery room beds. The amount of time necessary to transport a patient from an operating room to a recovery room is fixed and independent of the patient. Similarly, both the amount of time to prepare an operating room for the next patient and the amount of time to prepare a recovery room bed for a new patient are fixed.</p>
<p>
All patients are officially scheduled for surgery at the same time, but the order in which they actually go into the operating rooms depends on the order of the patient roster. A patient entering surgery goes into the lowest numbered operating room available. For example, if rooms 2 and 4 become available simultaneously, the next patient on the roster not yet in surgery goes into room 2 and the next after that goes into room 4 at the same time. After surgery, a patient is taken to the available recovery room bed with the lowest number. A recovery room bed is only available if the preparation is already finished when the patient leaves surgery. If two patients emerge from surgery at the same time, the patient with the lower surgery room number will be the first assigned to a recovery room bed.</p>
<h3>Input</h3>
<p>
The input file contains data for several simulation runs. Each run is separated by a blank line. All numeric data in the input file are integers, and successive integers on the same line are separated by blanks. The first line of each run is the set of hospital configuration parameters to be used for this run. The parameters are, in order:</p>
<p>
</p><ul>
<li>Number of operating rooms  (maximum of 10)</li>
<li>Number of recovery room beds (maximum of 30)</li>
<li>Starting hour for 1st surgery of day (based on a 24-hour clock)</li>
<li>Minutes to transport patient from operating room to recovery room</li>
<li>Minutes to prepare operating room for next patient</li>
<li>Minutes to prepare recovery room bed for next patient</li>
<li>Number of surgery patients for the day (maximum of 100)</li>
</ul><p></p>
<p>
This initial configuration data will be followed by pairs of lines of patient data as follows:</p>
<p></p><ul>
<li>Line 1:  Last name of patient (maximum of 8 characters)</li>
<li>Line 2: Minutes required for surgery Minutes required in the recovery room</li>
</ul>
<p></p>
<p>
Patient records in the input file are ordered according to the patient roster, which determines the order in which patients are scheduled for surgery. The number of recovery room beds specified in any configuration will be sufficient to handle patients arriving from surgery (No queuing of patients for recovery room beds will be required). Computed times will not extend past 24:00.</p>
<h3>Output</h3>
<p>Correct output shows which operating room and which recovery room bed is used by each patient, and the time period that the patient uses the room and bed along with a summary of the utilization of hospital facilities for that day. The output file consists of several sets of two tables each describing the results of the simulation run. The first table is in columnar form with appropriate column labels to show the number of each patient (in the order the patient roster), the patient's last name, the operating room number, the time surgery begins and ends, the recovery bed number and the time the patient enters and leaves the recovery room bed.</p>
<p>
The second table will also be in columnar form with appropriate column labels summarizing the utilization of operating rooms and recovery room beds. This summary indicates the facility type (room or bed), the facility number, the number of minutes used and percentage of available time utilized. Available time is defined as the time in minutes from the starting time for 1st surgery of day to the ending time of the last patient in a recovery room bed. Print a blank line after each run. Follow the output format shown on sample output.</p>

<h3>Example</h3>

<pre><b>Input:</b>

5 12 07 5 15 10 16
Jones
28 140
Smith
120 200
Thompson
23 75
Albright
19 82
Poucher
133 209
Comer
74 101
Perry
93 188
Page
111 223
Roggio
69 122
Brigham
42 79
Nute
22 71
Young
38 140
Bush
26 121
Cates
120 248
Johnson
86 181
White
92 140

<b>Output:</b>

 Patient          Operating Room          Recovery Room
 #  Name     Room#  Begin   End      Bed#  Begin    End
 ------------------------------------------------------
 1  Jones      1    7:00    7:28      3    7:33    9:53
 2  Smith      2    7:00    9:00      1    9:05   12:25
 3  Thompson   3    7:00    7:23      2    7:28    8:43
 4  Albright   4    7:00    7:19      1    7:24    8:46
 5  Poucher    5    7:00    9:13      5    9:18   12:47
 6  Comer      4    7:34    8:48      4    8:53   10:34
 7  Perry      3    7:38    9:11      2    9:16   12:24
 8  Page       1    7:43    9:34      6    9:39   13:22
 9  Roggio     4    9:03   10:12      9   10:17   12:19
10  Brigham    2    9:15    9:57      8   10:02   11:21
11  Nute       3    9:26    9:48      7    9:53   11:04
12  Young      5    9:28   10:06      3   10:11   12:31
13  Bush       1    9:49   10:15     10   10:20   12:21
14  Cates      3   10:03   12:03      8   12:08   16:16
15  Johnson    2   10:12   11:38      4   11:43   14:44
16  White      5   10:21   11:53      7   11:58   14:18

Facility Utilization
Type  # Minutes  % Used
-------------------------
Room  1     165   29.68
Room  2     248   44.60
Room  3     258   46.40
Room  4     162   29.14
Room  5     263   47.30
Bed   1     282   50.72
Bed   2     263   47.30
Bed   3     280   50.36
Bed   4     282   50.72
Bed   5     209   37.59
Bed   6     223   40.11
Bed   7     211   37.95
Bed   8     327   58.81
Bed   9     122   21.94
Bed  10     121   21.76
Bed  11       0    0.00
Bed  12       0    0.00

</pre>