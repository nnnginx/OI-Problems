<p>
	The Classical Maya civilization developed in what is today southern Mexico, 
	Guatemala, Belize and northern Honduras. During its height they developed a 
	sophisticated system for time keeping which they used both to record history 
	and for divinatory rituals. Their calendar consisted of 3 components. the 
	Tzolkin, the Haab and the Long Count.
</p>
<p>
	For divinatory purposes the Maya used the Tzolkin which was composed of 20 day 
	names to which numeric coefficients from 1 to 13 were attached giving a total 
	of 260 distinct combinations. This is the size of the Tzolkin, or ritual, year. 
	From Spanish colonial sources, we know the names of the days: <tt>Imix, Ik, Akbal, 
		Kan, Chikchan, Kimi, Manik, Lamat, Muluk, Ok, Chuen, Eb, Ben, Ix, Men, Kib, 
		Kaban, Etznab, Kawak, Ajaw</tt>. The sequence of days developed as follows 
	(starting for example at 9 Imix):
	</p><pre>9 Imix, 10 Ik, 11 Akbal, 12 Kan, 13 Chikchan, 1 Kimi, 2 Manik, ...</pre>
<p></p>
<p>
	The Haab calendar was an astronomical one. It had 365 days divided into 19 
	months each with 20 days, except the last one which had only 5 days. In a 
	manner similar to the Tzolkin each month name had a number from 1 to 20 
	indicating the day number within the month. Again, from Spanish colonial 
	sources, we know the names of the months: <tt>Pohp, Wo, Sip, Zotz, Sek, Xul, 
		Yaxkin, Mol, Chen, Yax, Sak, Keh, Mak, Kankin, Muan, Pax, Kayab, Kumku, Wayeb</tt>. 
	The month Wayeb had just 5 days and was considered an unlucky time of the year.
</p>
<p>
	The Tzolkin and Haab were combined in the inscriptions to create the Calendar 
	Round, combining the 260 day cycle of the Tzolkin and the 365 day cycle of the 
	Haab. A typical Calendar Round date in the inscriptions might be. 3 Lamat 6 
	Pax. Note that not all of the combination of days, months and coefficients are 
	possible.
</p>
<p>
	A typical sequence of days in the Calendar Round (starting for example at 3 
	Lamat 6 Pax):
	</p><pre>3 Lamat 6 Pax, 4 Muluk 7 Pax, 5 Ok 8 Pax, 6 Chuen 9 Pax, 7 Eb 10 Pax, 
8 Ben 11 Pax, 9 Ix 12 Pax, 10 Men 13 Pax, 11 Kib 14 Pax, 12 Kaban 15 Pax, 
13 Etznab 16 Pax, 1 Kawak 17 Pax, 2 Ajaw 18 Pax, 3 Imix 19 Pax, 4 Ik 20 Pax, 
5 Akbal 1 Kayab, 6 Kan 2 Kayab, ... 
</pre>
<p></p>
<p>
	Finally, at the beginning of the Classic Period (AD 200 - 900), the Maya 
	developed an absolute calendar called Long Count which counted the days from a 
	fixed date in the past (the date when the current world was created according 
	to Maya belief). Dates in the Long Count are given (for simplicity) in 5-tuples 
	of the form. 9.2.3.4.5. Such a date one reads "9 baktuns 2 katuns 3 tuns 4 
	winals 5 kins since the zero date". A "kin" is just one day. A winal is a group 
	of 20 days. A tun is a group of 18 winals (thus a tun has 20*18 = 360 days, 5 
	days short of a year). From here on all units come in multiples of 20. Thus a 
	katun is equal to 20 tuns (almost 20 years) and a baktun means 20 katuns 
	(almost 400 years). Thus 9.2.3.4.5 really means "9*144000+2*7200+3*360+4*20+5 
	days since the zero date". Note that for every Long Count date b.k.t.w.i we 
	have 0 &lt;= k &lt; 20; 0 &lt;= t &lt; 20; 0 &lt;= w &lt; 18; 0 &lt;= i &lt; 
	20. Given the periodicity of the Calendar Round, a legal date such as 3 Lamat 6 
	Pax has multiple occurrences in the Long Count. Thus, one difficulty in reading 
	inscriptions is in establishing a date for the inscription when the date is 
	given only in terms of a Calendar Round (very common). In this case one must 
	compute "all" the possible Long Count dates associated with the particular 
	Calendar Round and based in some other context information deduce (for example, 
	the text mentions a king for which other dates are known) which one applies.
</p>
<p>
	We limit our interest to the Long Count dates in the baktuns 8 and 9 (they 
	cover all the Classic Period). We know that the Long Count date 8.0.0.0.0 fell 
	on the Calendar Round 9 Ajaw 3 Sip.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads a Calendar Round date,
		</li><li>
		computes all Long Count dates in the baktuns 8 and 9 for the given Calendar 
		Round date if this date is legal,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input contains exactly one positive integer d equal to 
	the number of data sets, 1 &lt;= d &lt;= 30. The data sets follow.
</p>
<p>
	Each data set consists of exactly one line that contains exactly one Calendar 
	Round date (maybe illegal). Tzolkin day number, Tzolkin day name, Haab day 
	number and Haab month name separated by single spaces.
</p>
<h3>Output</h3>
<p>
	For every data set your program must output an ascending sequence of Long Count 
	dates computed for a given Calendar Round date. The first line of the output 
	for the given input set should contain exactly one integer n equal to the 
	length of the sequence (0, if the input date is illegal).
</p>
<p>
	Each of the next n lines should contain exactly one Long Count date specified 
	by exactly 5 integers (meaning the numbers of baktuns, katuns, tuns, winals and 
	kins respectively) separated by single dots.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2 
3 Lamat 6 Pax 
1 Ajaw 9 Chen 

<b><tt>Sample output:</tt></b>
15 
8.0.17.17.8 
8.3.10.12.8 
8.6.3.7.8 
8.8.16.2.8 
8.11.8.15.8 
8.14.1.10.8 
8.16.14.5.8 
8.19.7.0.8 
9.1.19.13.8 
9.4.12.8.8 
9.7.5.3.8 
9.9.17.16.8 
9.12.10.11.8 
9.15.3.6.8 
9.17.16.1.8 
0 

</pre>