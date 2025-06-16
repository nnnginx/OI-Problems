<p style="text-align: justify;">During his last sabbatical, professor M. A. Ya made a surprising discovery about the old Maya calendar. From an old knotted message, professor discovered that the Maya civilization used a 365 day long year, called&nbsp;<em>Haab</em>, which had 19 months. Each of the first 18 months was 20 days long, and the names of the months were&nbsp;<em>pop, no, zip, zotz, tzec, xul, yoxkin, mol, chen, yax, zac, ceh, mac, kankin, muan, pax, koyab, cumhu</em>. Instead of having names, the days of the months were denoted by numbers starting from 0 to 19. The last month of Haab was called&nbsp;<em>uayet</em>&nbsp;and had 5 days denoted by numbers 0, 1, 2, 3, 4. The Maya believed that this month was unlucky, the court of justice was not in session, the trade stopped, people did not even sweep the floor.</p>
<p style="text-align: justify;">For religious purposes, the Maya used another calendar in which the year was called&nbsp;<em>Tzolkin</em>&nbsp;(holly year). The year was divided into thirteen periods, each 20 days long. Each day was denoted by a pair consisting of a number and the name of the day. They used 20 names:&nbsp;<em>imix, ik, akbal, kan, chicchan, cimi, manik, lamat, muluk, ok, chuen, eb, ben, ix, mem, cib, caban, eznab, canac, ahau</em>&nbsp;and 13 numbers; both in cycles.</p>
<p style="text-align: justify;">Notice that each day has an unambiguous description. For example, at the beginning of the year the days were described as follows:</p>
<p style="text-align: justify;"><em>1 imix, 2 ik, 3 akbal, 4 kan, 5 chicchan, 6 cimi, 7 manik, 8 lamat, 9 muluk, 10 ok, 11 chuen, 12 eb, 13 ben, 1 ix, 2 mem, 3 cib, 4 caban, 5 eznab, 6 canac, 7 ahau</em>, and again in the next period&nbsp;<em>8 imix, 9 ik, 10 akbal...</em></p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">Years (both Haab and Tzolkin) were denoted by numbers 0, 1, ..., where the number 0 was the beginning of the world. Thus, the first day was:</p>
<p style="text-align: justify;">Haab:&nbsp;<code>0. pop 0</code></p>
<p style="text-align: justify;">Tzolkin:&nbsp;<code>1 imix 0</code></p>
<p style="text-align: justify;">Help professor M. A. Ya and write a program for him to convert the dates from the Haab calendar to the Tzolkin calendar.</p>
<p style="text-align: justify;">&nbsp;</p>
<h2>Input</h2>
<p>The date in Haab is given in the following format:</p>
<p><em>NumberOfTheDay. Month Year</em>&nbsp;</p>
<p>The first line of the input file contains the number of the input dates in the file. The next&nbsp;<em>n</em>&nbsp;lines contain&nbsp;<em>n</em>&nbsp;dates in the Haab calendar format, each in separate line. The year is smaller then 5000.</p>
<p>&nbsp;</p>
<h2>Output</h2>
<p>The date in Tzolkin should be in the following format:</p>
<p><em>Number NameOfTheDay Year</em></p>
<p>The first line of the output file contains the number of the output dates. In the next&nbsp;<em>n</em>&nbsp;lines, there are dates in the Tzolkin calendar format, in the order corresponding to the input dates.</p>
<p><strong><span style="font-size: small;">Sample Input</span></strong></p>
<pre>3
10. zac 0
0. pop 0
10. zac 1995</pre>
<p><strong><span style="font-size: small;">Sample Output</span></strong></p>
<pre>3
3 chuen 0
1 imix 0
9 cimi 2801</pre>