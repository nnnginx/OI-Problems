<p>
The sadists who design problems for ACM programming contests often like to include the abbre-
viation ¡°ACM¡± somewhere in their problem descriptions. Thus, in years past, the World Finals
has had problems involving ¡°Apartment Construction Management,¡± the ¡°Atheneum of Culture and
Movies,¡± the ¡°Association of Cover Manufacturers,¡± ¡°ACM Airlines,¡± the ¡°Association for Computa-
tional Marinelife,¡± and even an insect named ¡°Amelia Cheese Mite.¡± However, the number of word
combinations beginning with A, C, and M that make sense is finite and the problem writers are starting
to run out of ideas (it¡¯s hard to think of problems about ¡°Antidisestablishmentarianistic Chthonian
Metalinguistics¡±). Fortunately, modern culture allows more flexibility in designing abbreviations ¡ª
consider, for example:

</p><p></p><p>
</p><pre>GDB ¡ª Gnu DeBugger
LINUX ¡ª either ¡°LINus¡¯s UniX¡± or ¡°LINUs¡¯s miniX¡± or ¡°Linux Is Not UniX¡±
SNOBOL ¡ª StriNg Oriented symBOlic Language
SPITBOL ¡ª SPeedy ImplemenTation of snoBOL
</pre>

<p></p><p>
The rules used in these examples seem to be:

</p><p></p><p>
</p><ul>
<li> Insignificant words (such as ¡°of¡±, ¡°a¡±, ¡°the¡±, etc.) are ignored.
</li><li> The letters of the abbreviation must appear, in the correct order, as an ordered sublist of the
letters in the significant words of the phrase to be abbreviated.
</li><li> At least one letter of the abbreviation must come from every significant word (multiple occurrences
of a letter are, of course, treated as distinct).
</li></ul>

<p></p><p>
Of course these rules are often broken in real life. For instance, RADAR is an abbreviation for ¡°RAdio
Detecting And Ranging¡±. Under our rules (assuming that ¡°and¡± is an insignificant word), this would
not be a valid abbreviation (however, RADR or RADRAN or DODGING would be valid). You have
been asked to take a list of insignificant words and a list of abbreviations and phrases and to determine
in how many ways each abbreviation can be formed from the corresponding phrase according to the
rules above.

</p><h3>Input</h3>
<p>
The input file consists of multiple scenarios. Each scenario begins with an integer 100 &gt;= <i>n</i> &gt;= 1 followed
by <i>n</i> insignificant words, all in lower case, one per line with no extra white space. (A line containing
0 indicates end of input.) Following this are one or more test cases for this scenario, one per line,
followed by a line containing the phrase ¡°LAST CASE¡±. Each line containing a test case begins with
an abbreviation (uppercase letters only) followed by a phrase (lowercase letters and spaces only). The
abbreviation has length at least 1 and the phrase contains at least one significant word. No input line
(including abbreviation, phrase, and spaces) will contain more than 150 characters. Within these limits,
however, abbreviations and phrase words may be any length.

</p><h3>Output</h3>
<p>
For each test case, output the abbreviation followed by either

<i>
</i></p><p></p><p><i>
is not a valid abbreviation

</i></p><p></p><p><i>
or

</i></p><p></p><p><i>
can be formed in i ways</i>

</p><p></p><p>
where <i>i</i> is the number of different ways in which the letters of the abbreviation may be assigned to the
letters in the phrase according to the rules above. The value of <i>i</i> will not exceed the range of a 32-bit
signed integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
and
of
ACM academy of computer makers
RADAR radio detection and ranging
LAST CASE
2
a
an
APPLY an apple a day
LAST CASE
0

<b>Output:</b>
ACM can be formed in 2 ways
RADAR is not a valid abbreviation
APPLY can be formed in 1 ways
</pre>