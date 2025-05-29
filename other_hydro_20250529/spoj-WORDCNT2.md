<div id="wordcnt2_problem_body" style="font-size:1.3em">
<div id="wordcnt2_problem_description">
<p style="text-align:right">¡°I have hated words and I have loved them, and I hope I have made them right.¡± ¨D Markus Zusak</p>
<p style="text-align:justify">We also love words, don¡¯t we? However, we are code poets, so, we love words in a different way. How about counting them? Yes, counting word seems to be a good thing and has a huge application in computer science. Well, counting may sometimes sound boring, but many hidden knowledge can be achieved from counting. For example, finding the most frequent word in vast collection of documents, which then in turns, can be used to classify those documents.</p>
<p style="text-align:justify">But fear not! We are not interested in large documents right now. In fact, in our extremely busy world, offline data processing algorithms are getting obsolete day by day. Instead of words in large files, we are now more interested in streams of words.</p>
<p style="test-align:justify">The idea is quite simple, your program will keep reading from a stream where new words are continuously being fed to your program, but due to limited storage, your program can only remember the latest K words. So, when (K+1)<sup>th</sup> word arrives, your program forgets the 1<sup>st</sup> word, when (k+2)<sup>th</sup> word arrives, your program forgets the 2<sup>nd</sup> word, and so on.</p>
<p style="text-align:justify">We want you to find the most frequent word over the latest K words each time a new word arrives.</p>
</div>
<div id="wordcnt2_input_format">
<h3 style="text-align:left;margin:30px 0px -8px 0px;">Input Format</h3>
<p style="text-align:justify">The first line of input will contain an integer T, which denotes the number of test cases. First line of each test case will contain two integers N and K, where N is the total number of words to be read, and K is the number of words that your program can remember. Each of the following N lines will contain a single word composed with only lowercase characters ¡®a¡¯ to ¡®z¡¯, at most 8 characters long.</p>
</div>
<div id="wordcnt2_output_format">
<h3 style="text-align:left;margin:30px 0px -8px 0px;">Output Format</h3>
<p style="text-align:justify">For each case, first print the case number, then for each of the words, print the most frequent word that appears within the last K words along with the frequency. If there are less than K words, then print the most frequent word among all of them. In case there is a tie, print the alphabetically smaller word. See sample input and output sections for more details.</p>
</div>
<div id="wordcnt2_constraints">
<h3 style="text-align:left;margin:30px 0px 0px 0px;">Constraints</h3>
<p style="margin:2px">1 ¡Ü T ¡Ü 20</p>
<p style="margin:2px">1 ¡Ü K ¡Ü N ¡Ü 10<sup>5</sup></p>
<p style="margin:2px">1 ¡Ü word-length ¡Ü 8</p>
</div>
<div id="wordcnt2_sample_input">
<h3 style="text-align:left;margin:30px 0px -8px 0px;">Sample Input</h3>
<pre>1
8 3
hello
hi
who
hi
hi
hello
who
when
</pre>
</div>
<div id="wordcnt2_sample_output">
<h3 style="text-align:left;margin:30px 0px -8px 0px;">Sample Output</h3>
<pre>Case 1:
hello 1
hello 1
hello 1
hi 2
hi 2
hi 2
hello 1
hello 1
</pre>
</div>
<div id="wordcnt2_explanation">
<h3 style="text-align:left;margin:30px 0px -8px 0px;">Explanation</h3>
<p style="text-align:justify">The following table shows a simulation of the program for the entry of each new word. Note, once the capacity of the program is full, i.e. equals to K, the program will start forgetting the oldest entry for each new entry. In other words, those words will not be taken into consideration anymore.</p>
<table style="border: 1px solid black; width: 100%; text-align: left;" border="0">
<tbody>
<tr>
<th style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 4px;">#</th> <th style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 4px;">New word in stream</th> <th style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 4px;">Words remembered by the program</th> <th style="border-bottom: 1px solid black; padding: 4px;">Most frequent word (Count)</th>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">1</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hello</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hello</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hello (1)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">2</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hello, hi</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hello (1)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">3</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">who</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hello, hi, who</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hello (1)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">4</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi, who, hi</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hi (2)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">5</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">who, hi, hi</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hi (2)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">6</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hello</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi, hi, hello</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hi (2)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">7</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">who</td>
<td style="border-right: 1px solid black; border-bottom: 1px solid black; padding: 2px;">hi, hello, who</td>
<td style="border-bottom: 1px solid black; padding: 2px;">hello (1)</td>
</tr>
<tr>
<td style="border-right: 1px solid black; padding: 2px;">8</td>
<td style="border-right: 1px solid black; padding: 2px;">when</td>
<td style="border-right: 1px solid black; padding: 2px;">hello, who, when</td>
<td style="padding: 2px;">hello (1)</td>
</tr>
</tbody>
</table>
</div>
<br><br></div>