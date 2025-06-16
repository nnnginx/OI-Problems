<p>For some years, quite a lot of work has been put into listening to electromagnetic radio signals received from space, in order to understand what civilizations in distant galaxies might be trying to tell us. One signal source that has been of particular interest to the scientists at Universit´e de Technologie Spatiale is the Nebula Stupidicus.
<br><br>
Recently, it was discovered that if each message is assumed to be transmitted as a sequence of integers a0, a1, ...an-1 the function f(k) = <img src="./23678/file/GqUm1ZKn.png"> (mod p) always evaluates to values 0 &lt;= f(k) &lt;= 26 for 1 &lt;= k &lt;= n, provided that the correct value of p is used. n is of course the length of the transmitted message, and the ai denote integers such that 0 &lt;= ai &lt; p. p is a prime number that is guaranteed to be larger than n as well as larger than 26. It is, however, known to never exceed 30 000.
<br><br>
These relationships altogether have been considered too peculiar for being pure coincidences, which calls for further investigation.
<br><br>
The linguists at the faculty of Langues et Cultures Extraterrestres transcribe these messages to strings in the English alphabet to make the messages easier to handle while trying to interpret their meanings. The transcription procedure simply assigns the letters a..z to the values 1..26 that f(k) might evaluate to, such that 1 = a, 2 = b etc. The value 0 is transcribed to ’*’ (an asterisk). While transcribing messages, the linguists simply loop from k = 1 to n, and append the character corresponding to the value of f(k) at the end of the string.
<br><br>
The backward transcription procedure, has however, turned out to be too complex for the linguists to handle by themselves. You are therefore assigned the task of writing a program that converts a set of strings to their corresponding Extra Terrestial number sequences.

</p><h3>Input</h3>
<p>On the first line of the input there is a single positive integer N, telling the number of test cases to follow. Each case consists of one line containing the value of p to use during the transcription of the string, followed by the actual string to be transcribed. The only allowed characters in the string are the lower case letters ’a’..’z’ and ’*’ (asterisk). No string will be longer than 70 characters.

</p><h3>Output</h3>
<p>For each transcribed string, output a line with the corresponding list of integers, separated by space, with each integer given in the order of ascending values of i.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
31 aaa
37 abc
29 hello*earth

<b>Output:</b>
1 0 0
0 1 0
8 13 9 13 4 27 18 10 12 24 15
</pre>