<p>Emoticons are used in chat and e-mail conversations to try to express the emotions that printed
words cannot. This may seem like a nice feature for many, but a lot of people find it really
annoying and wants to get rid of emoticons.

</p><p></p><p>
George is one of those people. He hates emoticons so bad, that he is preparing a plan to
remove all emoticons from all e-mails in the world. Since you share his visionary plans, you are
preparing a special program to help him.

</p><p></p><p>
Your program will receive the list of emoticons to proscribe. Each emoticon will be a string of
characters not including any whitespace. You will also receive several lines of text. What you
need to do is change some characters of the text into spaces to ensure no emoticon is left on
the text. For an emoticon to be considered to appear in the text it has to appear in a single
line and be made of consecutive characters.

</p><p></p><p>
To help George��s plan remain secret as long as possible, you need to do your job with the
minimum possible amount of character changes.

</p><h3>Input</h3>
<p>The input file contains several test cases. Each test case consists of several lines. The first
line of each test case will contain two integers separated by a single space: N, the number of
emoticons to proscribe, and M, the number of lines the text has. The next N lines contain one
emoticon each, a non-empty string of at most 15 characters. Each of the last M lines of the
test case contains a line of text of at most 80 characters. You can assume 1 &lt;= N,M &lt;= 100.

</p><p></p><p>
Valid input characters for emoticons are uppercase and lowercase letters, digits and the symbols
��!?.,:;-_��#$%&amp;/=*+(){}[]�� (quotes for clarity). Each line of the text may contain the same
characters with the addition of the space character.

</p><p></p><p>
The input is terminated by N = M = 0.

</p><h3>Output</h3>
<p>For each test case, output exactly one line containing a single integer that indicates the minimum
number of changes you need to make to the entire text to ensure no emoticon on the list appears
in it.

</p><h3>Example</h3>

<pre><b>Input:</b>
4 6
:-)
:-(
(-:
)-:
Hello uncle John! :-) :-D
I am sad or happy? (-:-(?
I feel so happy, my head spins
(-:-)(-:-)(-:-)(-:-) :-) (-: :-)
but then sadness comes :-(
Loves you, Joanna :-)))))
3 1
:)
):
))
:):)):)):)):(:((:(((:):)
0 0

<b>Output:</b>
11
8
</pre>