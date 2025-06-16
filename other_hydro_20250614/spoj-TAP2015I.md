<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>In the novel <em>"A for Andromeda"</em>, by Fred Hoyle and John Elliot, a civilization from a planet in orbit around a star in the constellation of Andromeda, 200 light years away from our Solar System, decides to colonize the galaxy. To avoid the long and costly interstellar travels, this civilization decides to perform the colonization at a distance, by sending a signal instead of ships (this signal contains instructions on how to build a supercomputer with an artificial intelligence capable of taking over the world of the unfortunate civilizations who build it, but that is not our problem for the moment).</p>
<p>One of the issues humans have to overcome in order to construct the supercomputer is the decoding of the signal. As it happens, the aliens send two messages in two different frequencies, repeating endlessly in each of them a code with <strong>N</strong> characters. For example, if <strong>N = 3</strong> and one of the codes is <strong>"<span style="font-family: 'courier new', courier;">abc</span>"</strong>, the alien message in the corresponding frequency will be <strong>"...<span style="font-family: 'courier new', courier;">cabcabcabcab</span>..."</strong>, where the ellipsis mean that the code is repeated infinitely both backwards and forwards. For this reason, the terrestrial stations receiving the signal are incapable of telling what the emitted code actually is, as there can be more than one code that is compatible with a given message. In our example, knowing that <strong>N = 3</strong> they could interpret that the code is any of three possibilities <strong>"<span style="font-family: 'courier new', courier;">abc</span>"</strong>, <strong>"<span style="font-family: 'courier new', courier;">bca</span>"</strong> and <strong>"<span style="font-family: 'courier new', courier;">cab</span>"</strong>.</p>
<p>Complicating matters even further, although both messages are composed solely of characters from the alphabet <strong>'<span style="font-family: 'courier new', courier;">a</span>'</strong> through <strong>'<span style="font-family: 'courier new', courier;">z</span>'</strong>, because they are transmitted in different frequencies there exists an ambiguity in the identification of the characters between them. Thus, if we let the characters be named <strong>c<sub>1</sub>&nbsp;= '<span style="font-family: 'courier new', courier;">a</span>'</strong>, <strong>c<sub>2</sub>&nbsp;= '<span style="font-family: 'courier new', courier;">b</span>'</strong>, and so on until <strong>c<sub>26</sub>&nbsp;= '<span style="font-family: 'courier new', courier;">z</span>'</strong>, it is possible that every occurrence of the character <strong>c<sub>i</sub></strong>&nbsp;in one of the messages is replaced by the character <strong>c<sub>考(i)</sub></strong>&nbsp;in the other message, where <strong>考(i)</strong> is an arbitrary permutation of the numbers from <strong>1</strong> to <strong>26</strong>. For instance, if we have <strong>考(1) = 24</strong>, <strong>考(2) = 25</strong> and <strong>考(3) = 26</strong> the code <strong>"<span style="font-family: 'courier new', courier;">abc</span>"</strong> in one of the frequencies will be turned in the other into <strong>"<span style="font-family: 'courier new', courier;">xyz</span>"</strong>, so that the corresponding message will be <strong>"...<span style="font-family: 'courier new', courier;">zxyzxyzxyzxy</span>..."</strong>.</p>
<p>You've been put in charge of decoding the alien signal, and your task is to determine the maximum length of a common substring that two codes compatible with the received messages can have. This is, you should find the maximum value <strong>K</strong> such that one of the messages is compatible with the code <strong>a<sub>1</sub>&nbsp;a<sub>2</sub>&nbsp;... a<sub>N</sub></strong>&nbsp;and the other is compatible with the code <strong>b<sub>1</sub>&nbsp;b<sub>2</sub>... b<sub>N</sub></strong>, and there exist <strong>i</strong> and <strong>j</strong> with <strong>0 ≒&nbsp;i</strong>, <strong>j&nbsp;≒&nbsp;N-K</strong> such that <strong>a<sub>i+k</sub>&nbsp;= b<sub>j+k</sub></strong>&nbsp;for <strong>k = 1, ..., K</strong> up to a permutation of the alphabet.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer <strong>N</strong> representing the length of the codes emitted by the aliens (<strong>1 ≒ N ≒ 1000</strong>). Each of the two following lines contains the description of the message received in a different frequency, in the form of a string of <strong>N</strong> characters from <strong>'<span style="font-family: 'courier new', courier;">a</span>'</strong> to <strong>'<span style="font-family: 'courier new', courier;">z</span>'</strong>. The received message is obtained repeating endlessly the corresponding string.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line containing an integer representing the maximum length of a common substring two codes which are compatible with the received messages can have.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3
abc
xyz
3
aab
cdd
4
abab
xyzw
4
xyzw
abab
18
imzbyqlgjwrvfspthe
rubihyvjnomqdznhat</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
3
2
2
16</span><span style="white-space: normal;">
</span></pre>