<p align="justify">Given a string of characters, we can permute the individual characters to   make new strings. If we can impose an ordering on the characters (say alphabetic   sequence), then the strings themselves can be ordered and any given permutation   can be given a unique number designating its position in that ordering. For   example the string `acab' gives rise to the following 12 distinct permutations: </p>
<div align="center">
  <table width="149" border="0">
    <tbody><tr>
      <td width="29">aabc</td>
      <td width="10">1</td>
      <td width="29">acab</td>
      <td width="10">5</td>
      <td width="29">bcaa</td>
      <td width="16">9</td>
    </tr>
    <tr>
      <td>aacb</td>
      <td>2</td>
      <td>acba</td>
      <td>6</td>
      <td>caab</td>
      <td>10</td>
    </tr>
    <tr>
      <td>abac</td>
      <td>3</td>
      <td>baac</td>
      <td>7</td>
      <td>caba</td>
      <td>11</td>
    </tr>
    <tr>
      <td>abca</td>
      <td>4</td>
      <td>baca</td>
      <td>8</td>
      <td>cbaa</td>
      <td>12</td>
    </tr>
  </tbody></table>
</div>
<p align="justify">Thus the string `acab' can be characterised in this sequence as 5. </p>
<p align="justify">Write a program that will read in a string and determine its position in the   ordered sequence of permutations of its constituent characters. Note that   numbers of permutations can get very large; however we guarantee that no string   will be given whose position is more than 2^31 = 2.147.483.647</p>
<h2>Input and Output </h2>
<p>Input will consist of a series of lines, each line containing one string.   Each string will consist of up to 30 lower case letters, not necessarily   distinct. Test cases a separated by empty lines. The file will be terminated by a line consisting of a single   #. </p>
<p>Output will consist of a series of lines, one for each line of the input.   Each line will consist of the position of the string in its sequence, right   justified in a field of width 10. </p>
<h2>Sample Input </h2>
<pre>bacaa
abc
cba

bacaa
abc
cba
#</pre>
<p> </p>
<h2>Sample Output </h2>
<pre>        15
         1
         6

        15
         1
         6
</pre>