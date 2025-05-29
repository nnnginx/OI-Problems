<p>Computer Scientists have a rough life. Due to the shortage of bright young minds like yourself, good programmers are mostly like famous movie stars. It's just like everyone wants to get their hands on your hard earned cash. The situation got so out of hand that you are faced by a lawsuit nearly every day of the year. Each lawsuit is filed by someone claiming alimonies for your alleged child. Luckily for you, you know pretty much about genetic sequences. You know that the human DNA sequence can be represented by a possibly <em>N</em> characters long string, containing only characters 'a' to 'z'. And you know that a similarity test of the DNA strings of the alleged child to your own can prove your innocence.</p>
<p>The only problem is that this does not only happen to you. As all labs are busy, testing needs at least a year. Still, not all hope is lost. You managed to get the information from one of the DNA labs on how to compute the probability of a genetic relationship between two DNA strings. If you could only help the DNA labs to test two DNA strings for a genetic relationship really fast, you could get the evidence you need for your own lawsuits.</p>
<p>A genetic relationship test, or GRT, requires some heavy computation on the DNA strings. They first acquire all similar regions within two DNA strings. We understand a region within a DNA string to be a consecutive interval within the DNA string. Regions <em>a[i..i+l]</em> (<em>0 ¡Ü i &lt; N-l</em>) and <em>b[j..j+l]</em> (<em>0 ¡Ü j &lt; N-l</em>) of DNA strings <em>a, b</em> are similar to each other, if <em>|a[i+k] - b[j+k]| ¡Ü  1</em> for <em>0 ¡Ü k ¡Ü l</em>. A GRT between two DNA sequences is positive, whenever the two DNA sequences have a similar region of at least one half the length of the DNA sequences.</p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases <em>C</em> (<em>0 &lt; C ¡Ü 1000</em>). The first line of each such test case holds an integer <em>N</em> (<em>1 ¡Ü N ¡Ü 1000</em>), denoting the length of the two DNA strings to be tested. The following two lines contain a string of <em>N</em> lower-case letters each, giving the two DNA substrings of the two persons to test.</p>
<h3>Output</h3>
<p>For each test case print one line. If the GRT is positive, print out <strong>POSITIVE</strong>. Print <strong>NEGATIVE</strong>, if the test fails.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
4
aaaa
bbcc
8
iacdefgh
abeaaaaa
8
iacdefgh
abeafaaa

<strong>Output:</strong>
POSITIVE
NEGATIVE
NEGATIVE
</pre>