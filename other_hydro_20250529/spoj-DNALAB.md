<p align="justify">Having started to build his own DNA lab just recently, the evil doctor Frankenstein is not quite
  up to date yet. He wants to extract his DNA, enhance it somewhat and clone himself. He has
  already figured out how to extract DNA from some of his blood cells, but unfortunately reading
  off the DNA sequence means breaking the DNA into a number of short pieces and analyzing those
  first. Frankenstein has not quite understood how to put the pieces together to recover the original<br>
sequence.</p>
<p align="justify">  His pragmatic approach to the problem is to sneak into university and to kidnap a number of
  smart looking students. Not surprisingly, you are one of them, so you would better come up with
a solution pretty fast.</p>
<p align="justify">  You are given a list of strings over the alphabet A (for adenine), C (cytosine), G (guanine), and T
  (thymine), and your task is to find the shortest string (which is typically not listed) that contains
  all given strings as substrings. If there are several such strings of shortest length, find the smallest
  in alphabetical/lexicographical order.<br>
</p>
<p align="justify"><strong>Input</strong><br>
  The fist line contains the number of scenarios. For each scenario, the first line contains the number
  n of strings with 1&lt;=n&lt;=15. Then these strings with 1 &lt;= length &lt;= 100 follow, one on each line,
  and they consist of the letters ¡®A¡¯, ¡®C¡¯, ¡®G¡¯, and ¡®T¡¯ only.<br>
</p>
<p align="justify"><strong>Output</strong><br>
  The output for every scenario begins with a line containing ¡°Scenario #i:¡±, where i is the number
  of the scenario starting at 1. Then print a single line containing the shortest (and smallest) string
  as described above. Terminate the output for the scenario with a blank line.<br>
</p>
<p align="justify"><strong>Sample Input</strong><br>
  1<br>
  2<br>
  TGCACA<br>
  CAT<br>
</p>
<p align="justify"><strong>Sample Output</strong><br>
</p>
<p align="justify">Scenario #1:<br>
  TGCACAT</p>