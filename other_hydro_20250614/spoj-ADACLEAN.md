<p>Ada the Ladybug has decided to do some "Spring Cleaning". As you might know, she keeps a TODO list. She is very sparing so she keeps all her activities as one string. You might get very confused while reading the string but she has a system - every activity has length exactly <strong>K</strong> characters. Sadly, as new activities were added to the list many duplicities appeared. Now it is time to find out how many <strong>unique</strong> activities are in her TODO list.</p>
<h3>Input</h3>
<p>First line contains <strong>T</strong>, number of test-cases.</p>
<p>Each test-case begins with <strong>N, K</strong>, <strong> 1 ¡Ü K ¡Ü N ¡Ü     10<sup>5</sup></strong>, length of string and length of activites respectively.</p>
<p>Next line consists of string of length <strong>N</strong>, consisting of lowercase letters.</p>
<p>The sum of lengths of strings among all test-cases won't exceed <strong>3*10<sup>5</sup></strong></p>
<h3>Output</h3>
<p>For each test-case, print the number of unique substrings of length <strong>K</strong></p>
<h3>Example Input</h3>
<pre>5
3 2
aaa
5 1
abcba
4 2
abac
10 2
abbaaaabba
7 3
dogodog
</pre>
<h3>Example Output</h3>
<pre>1
3
3
4
4
</pre>