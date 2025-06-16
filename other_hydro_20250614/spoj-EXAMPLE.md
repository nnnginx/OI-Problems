<p>As you may have probably noticed a problem statement in a programming contest consists of several
sections. The most important section is, of course, the "Example" section. Some seasoned contestants even
start reading the problem statement from the examples. And, unfortunately, the least read section is the
problem description section. It is quite disappointing for the problem authors because they feel that their
writing skills are largely wasted.</p>
<p>So the authors decided to describe examples in the same language, as the rest of the problem statement using
the following rules.</p>
<div align="justify">
<ul>
<li>
Natural integer numbers shall be written in plain English. The numbers shall be less than one hundred. The
designator number shall be written before numbers, except when the corresponding number is used as a
<b>repetition factor</b>. For example, <i>number zero</i>, <i>number sixteen</i>, or <i>number sixty one</i>.
</li><li>
Sequences of characters (strings) shall be written either in quotes, or in apostrophes, for example <i>"John's pen"</i>,
or <i>'5" tall'</i>. Note, that ' may be used in strings enclosed in " and vice versa. The designator string
shall be written before strings, for example <i>string 'Hello'</i>.
</li><li>
The designator <i>space</i> denotes one space character.
</li><li>
A number, string or space may be prefixed with a <b>repetition factor</b>. The repetition factor is a number greater
than one. The designator after the repetition factor is written in plural form. For example, <i>four numbers five</i>, or <i>six strings 'A'</i>. If the repetition factor is used for numbers, the numbers are separated with one space character. So, the former example means <i>5 5 5 5</i>, but the latter example <i>AAAAAA</i>.
</li><li>
Let the numbers, strings and spaces with possible repetition factors be called <b>fragments</b>. Fragments may be
organized into <b>sequences</b> using the <i>followed by</i> copulative. For example, <i>number five followed by number six</i>. One implicit space character is assumed between numbers, a number and a string, and a string
and a number so the example above means <i>5 6</i>.
</li><li>
An example is described line by line. The first line is always described as <i>The first line...</i>. The following
lines are described either as <i>The next line...</i> or as <i>The next # lines...</i>, where <i>#</i> is a number greater
than one. Empty lines are described as <i>is empty</i> or <i>are empty</i>. Other lines are described as <i>contains</i>
or <i>contain</i> followed by sequences. The first letter of a sentence is capitalized. The sentence is terminated by
a full stop (<b>.</b>). The full stop is not separated by space from the preceding word, but is separated by at least one
space from the next word.
</li></ul>
</div>
<h3>Input</h3>
<p>The input contains a free-flow text describing an example. Words are separated by an arbitrary number of
spaces and newlines. There are no whitespace characters after the last full stop. The total size of the input
will be no greater than 1 MB.</p>
<h3>Output</h3>
<p>The output should contain the decoded example. The total size of the output shall be no greater than 1 MB.</p>
<h3>Example</h3>
<pre><b>Input:</b>
The first line contains four
numbers twenty eight. The next
line is empty. The next two
lines contain six strings '-'.
The next line contains number
four followed by number seventy
seven followed by string 'meat'
followed by three strings "!".

<b>Output:</b>
28 28 28 28

------
------
4 77 meat!!!

</pre>