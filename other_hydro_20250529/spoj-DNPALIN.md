<p>C-3PO is an expert in pretty much every language. His conversation with R2-D2 are always fun to
observe un that R2-D2 speaks in Droid, C-3PO speak in English, and they understand each other
perfectly! Anyway, humans and droids both enjoy playing word games. A palindrome is a word or
sequence of one or more letters that reads the same forwards and backwards. A near palindrome is
a word or sequence that can be changed to or kept a palindrome by changing exactly one letter to a
different letter. For example. BAT is a near palindrome, since changing the T to a B woluld make
the word a palindrome: BAB. PEEP is not a near palindrome: although PEEP is palindrome,
changing any letter would remove its palindrome status. A double near palindrome is a word or
sequence that consist of two near palindromes concatenated together. For example, BATMAN is
a double near palindrome, since BAT and MAN are both near palindromes. Given a list of words,
you are to determine wich words are double near palindromes and wich are not.


</p><h3>Input</h3>
<p>The input consists of one or more words. All words (except the last) will be inclusively between 1
and 25 letters long and will consist of entirely of capital letters. The last word will be *END* and
is not be processed; it simply indicates the end of the input. There may be any number of spaces
and <eol> characters before, after, and between words.


</eol></p><h3>Output</h3>
<p>The output cases are to appear in the same order in wich they appear in the input. For each input
case, you are to print either w is a double near palindrome. or w is not a double near
palindrome. wichever is appropriate, where w is the input word. Exactly one <eol> should follow
each output case (meaning there should be no blank lines in the output).


</eol></p><h3>Example</h3>

<pre><b>Input:</b>
BATMAN
CONSTANTINOPLE
*END*

<b>Output:</b>
BATMAN is a double near palindrome.
CONSTANTINOPLE is not a double near palindrome.

</pre>