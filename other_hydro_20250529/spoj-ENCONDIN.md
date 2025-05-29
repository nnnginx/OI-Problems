<p>

Your task is to write a program that performs a simple form of run-length encoding, as described by the rules below.

</p><p>

Any sequence of between 2 to 9 identical characters is encoded by two characters.
The first character is the length of the sequence, represented by one of the characters <code>2</code> through <code>9</code>.
The second character is the value of the repeated character.
A sequence of more than 9 identical characters is dealt with by first encoding 9 characters, then the remaining ones.

</p><p>

Any sequence of characters that does not contain consecutive repetitions of any characters is represented by a <code>1</code> character followed by the sequence of characters, terminated with another <code>1</code>.
If a <code>1</code> appears as part of the sequence, it is escaped with a <code>1</code>, thus two <code>1</code> characters are output.

</p><h3>Input Specification</h3><p>

The input consists of letters (both upper- and lower-case), digits, spaces, and punctuation.
Every line is terminated with a newline character and no other characters appear in the input.

</p><h3>Output Specification</h3><p>

Each line in the input is encoded separately as described above.
The newline at the end of each line is not encoded, but is passed directly to the output.

</p><h3>Sample Input</h3><p>

</p><pre>AAAAAABCCCC
12344
</pre>

<h3>Sample Output</h3><p>

</p><pre>6A1B14C
11123124
</pre>