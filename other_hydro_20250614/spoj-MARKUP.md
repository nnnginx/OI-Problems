<p>

Mark-up languages are computer languages that assist in the formatting
of text files.  Special keywords are used to mark the text to allow
control of fonts, page styles, paragraph styles, etc.  TeX, troff,
and HTML are examples of mark-up languages. </p><p>

Spell checking can be difficult to adapt to these special texts.  In
general, special processors or spell checkers must be created in order
to accommodate mark-up languages.  A special processor would recognize
the mark-up language and strip it from the text so that the ``plain''
text could then be processed by a spell checker.  For this problem,
you are to write such a processor for a small mark-up language so
that the output of your program will be the plain text without the
mark-ups. </p><p>

The mark-up language to consider is one which allows the modification
of fonts within the text.  Each markup command will be preceded by a
<samp>\</samp> character.  If the letter following the <samp>\</samp>
character is not a recognized command from the table below then the
character following the <samp>\</samp> is printed as part of the plain
text.  For instance, the mark-up <samp>\\</samp> can be used to print
a single <samp>\</samp>. </p><p>

</p><table cellspacing="5">

<tbody><tr><td> 
</td><td valign="baseline"><pre>\b</pre>
</td><td> 
</td><td valign="baseline">toggle bold font on/off (default state is off)
</td></tr><tr>

<td> 
</td><td valign="baseline"><pre>\i</pre>
</td><td> 
</td><td valign="baseline">toggle italics font on/off (default state is off)
</td></tr><tr>

<td> 
</td><td valign="baseline"><pre>\s</pre>
</td><td> 
</td><td valign="baseline">set font size; the s is immediately followed by an
optional number; if the number is missing then the command will
restore the previous size
</td></tr><tr>

<td> 
</td><td valign="baseline"><pre>\*</pre>
</td><td> 
</td><td valign="baseline">toggle processing of mark-ups on/off; if
processing is toggle off then mark-ups are considered to be literal
text (default state is on)
</td></tr><tr>

</tr></tbody></table>

The number following the <samp>\s</samp> command can have a decimal
point so 12, 9.5, 11., and .5 should all be recognized as valid
numbers. <p>

The input file will be plain text containing mark-ups from the
language above.  At the start, processing of mark-ups should be on.
The file should be processed until the end-of-file is encountered. </p><p>

A sample input file is shown here: </p><p>

</p><pre>\s18.\bMARKUP sample\b\s

\*For bold statements use the \b command.\*

If you wish to \iemphasize\i something use the \\i command.

For titles use \s14BIG\s font sizes, 14 points usually works well.

Remember that all of the commands toggle except for the \\s command.
</pre>

<p>The following output file should be produced from the above sample input: </p><p>

</p><pre>MARKUP sample

For bold statements use the \b command.

If you wish to emphasize something use the \i command.

For titles use BIG font sizes, 14 points usually works well.

Remember that all of the commands toggle except for the \s command.
</pre>