<p>After teaching guitar to Jimmy Page (Led Zeppelin Band Guitarist), Sir Jadeja has decided to do something new. Sir Jadeja took out his guitar and started playing a melody he composed when he was 2 months old.</p>

<p>The guitar as usual has 6 strings denoted by numbers through 1 to 6. Each string is divided into P frets denoted by numbers 1 to P. A melody is a sequence of tones, where each tone is produced by picking a string pressed on a specific fret (for example: 4th string pressed on 8th fret). If a string is pressed on several frets, the produced tone will be the one corresponding to the highest of those frets. For instance, if the 3rd string is already pressed on the 5th fret, and the tone which corresponds to the 7th fret is to be produced, the string can be pressed on the 7th fret and picked without releasing the 5th fret. If a tone that corresponds to the 2nd fret on the same string is to be produced next, it is necessary to release both 5th and 7th frets and only then press 2nd.</p>

<p>Sir Jadeja feeling tired wants to play the melody with minimum number of finger movements. Note that press or release a single fret counts as one finger move. String picking is not a finger move, but rather a guitar pick move and should not be counted. Remember that picking a string with not affect frets being pressed on other string. You can assume that Sir Jadeja has enough fingers to press all the frets on all string at the same time (yes, that many).</p>

<h3>Input:</h3>
<p>First line contains two integers: N (N &lt;= 500000) and P (2 &lt;= P &lt;= 300000). N denotes number of tones in the melody and P denotes number of frets. The next N lines describe the fields for the corresponding tones: the number of the string and the number of the fret, respectively. Tones must be played in the order they are described.</p>

<h3>Output:</h3>
<p>Print a single integer: minimum number of finger movements that need to be made.</p>

<h3>Samples</h3>

<pre><u>INPUT 1:</u>
5 15 
2 8 
2 10 
2 12 
2 10 
2 5 

<u>OUTPUT 1:</u>
7

<u>INPUT 2:</u>
8 15 
2 8 
2 10 
2 12
3 7 
2 10
3 5 
2 5
3 3

<u>OUTPUT 2:</u>
12
</pre>

<h3>Explanation:</h3>
<p>For set 1: All the tones played are produced by picking the 2nd string . First the frets 8, 10, 12 are pressed in order(three movements). Then the 12th fret is released to produce the second tone again (fourth movement). Finally the fifth fret is pressed followed by the release of frets 10 and 12( 5th, 6th and 7th ).</p>